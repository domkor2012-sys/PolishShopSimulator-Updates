# Wydanie kolejnej wersji

1. Zbuduj i przetestuj finalny Windows export gry. Zapisz wersję `major.minor.patch`, np. `0.13.3`.
2. Umieść pliki eksportu w osobnym folderze. Główny EXE w paczce musi mieć nazwę `PolishShopSimulator.exe`; jeśli Godot używa zewnętrznego PCK, nazwij go `PolishShopSimulator.pck`.
3. Spakuj **same pliki gry** do `PolishShopSimulator-vX.Y.Z-Windows.zip`. Nie dodawaj source ani save'ów.
4. Policz SHA-256 ZIP i dokładny rozmiar w bajtach, np. `Get-FileHash ... -Algorithm SHA256` i `(Get-Item ...).Length`.
5. Utwórz GitHub Release z tagiem `vX.Y.Z` i dodaj ZIP jako asset. Opcjonalnie dodaj nowy EXE launchera jako osobny asset.
6. Zaktualizuj `version.json`: `version`, `release_name`, `download_url`, `sha256`, `size_bytes`, `release_notes`, `channel`. `download_url` musi być HTTPS i wskazywać dokładnie opublikowany ZIP.
7. Zaktualizuj `releases/SHA256SUMS.txt`, commituj i pushuj manifest do gałęzi `main`.
8. Sprawdź HTTP 200 dla publicznego URL manifestu i assetu oraz wykonaj lokalny test aktualizacji launchera na kopii instalacji.

Launcher porównuje wersje liczbowo; kanał stable ignoruje manifest beta. Najpierw opublikuj ZIP, potem nowy manifest, aby użytkownicy nie zobaczyli aktualizacji z brakującym plikiem.
