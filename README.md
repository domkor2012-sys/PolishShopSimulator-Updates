# Polish Shop Simulator — feed aktualizacji

Repozytorium zawiera manifest `version.json`, sumę SHA-256, dokumentację i przykładowy workflow. Paczka Windows i launcher są udostępniane jako pliki GitHub Releases. Kod gry **nie musi być publiczny**; repozytorium służy jako publiczny feed aktualizacji.

Repo aktualizacji: `domkor2012-sys/PolishShopSimulator-Updates`. Manifest jest dostępny pod `https://raw.githubusercontent.com/domkor2012-sys/PolishShopSimulator-Updates/main/version.json`. Wzór konfiguracji launchera jest w `launcher/launcher_config.example.json`. ZIP gry oraz launcher są publikowane jako GitHub Release assets, nie jako pliki Git.

Aktualna paczka jest rzeczywista i ma hash zapisany w `version.json` oraz `releases/SHA256SUMS.txt`. Kolejne wydania opisuje `RELEASE_GUIDE.md`. Feed musi pozostać publicznie dostępny, ponieważ launcher v1 nie ma mechanizmu logowania do GitHuba.
