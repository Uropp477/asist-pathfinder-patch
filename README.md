# mineflayer-pathfinder 2.4.5 — community patch

Fixy zebrane i przetestowane w projekcie `asist` (autonomiczny bot do Minecrafta, Paper 1.21.11):

- **Liście (`*_leaves`) są tanie do zniszczenia** — bot przecina las zamiast stać w miejscu lub robić ogromne objazdy (fix na problem z issue #222).
- **Otwarte drzwi** — poprawiony punkt docelowy przy drzwiach (bot nie blokuje się na skrzydle).
- **Klapki (trapdoor)** — otwieranie zamiast niszczenia, przechodzenie przez otwarte.
- **Pnącza (vine, weeping/twisting/cave vines)** — traktowane jako wspinaczkowe.
- **Próg "arrived" 0.35 → 0.175** — mniej zacinania na krawędziach bloków.
- **Lawa** — bot ucieka z lawy, zamiast omijać ją, gdy w niej stoi.

Część zmian inspirowana repo [mindcraft-bots/mindcraft](https://github.com/mindcraft-bots/mindcraft) (MIT).

## Jak użyć

```bash
npm install patch-package --save-dev
# wrzuć ten plik do: patches/mineflayer-pathfinder+2.4.5.patch
# dodaj do package.json: "postinstall": "patch-package"
npm install
