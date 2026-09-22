# Polish Shop Simulator — feed aktualizacji

Ten folder zawiera manifest `version.json`, paczkę Windows, sumę SHA-256, launcher i przykładowy workflow. Kod gry **nie musi być publiczny**. Repozytorium może służyć wyłącznie jako publiczny feed aktualizacji i miejsce plików GitHub Releases.

Repo aktualizacji: `domkor2012-sys/PolishShopSimulator-Updates`. Manifest jest dostępny pod `https://raw.githubusercontent.com/domkor2012-sys/PolishShopSimulator-Updates/main/version.json`. Wzór konfiguracji launchera jest w `launcher/launcher_config.example.json`. ZIP gry oraz launcher są publikowane jako GitHub Release assets, nie jako pliki Git.

Aktualna paczka jest rzeczywista i ma hash zapisany w `version.json` oraz `releases/SHA256SUMS.txt`. Kolejne wydania opisuje `RELEASE_GUIDE.md`. Feed musi pozostać publicznie dostępny, ponieważ launcher v1 nie ma mechanizmu logowania do GitHuba.
