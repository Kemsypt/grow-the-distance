# Grow the Distance

**Every step grows your world.**

A cosy real-world walking and farming game, previously called Hearthstride.
This is its own repository and website, separate from Luce’s Pokémon project.

## Source and publishing

`source.zip` contains the full Flutter source, Android project, assets and tests.
Extract it to work on the game locally. The publishing workflow extracts that same source, runs the tests, compiles the renamed browser app, and deploys it to GitHub Pages on every push to `main`.

In Settings → Pages, the publishing source should be **GitHub Actions**.

To update the game, replace `source.zip` with the updated project contents (pubspec.yaml at the archive root). The deployment workflow is stored separately in `.github/workflows/pages.yml`.

## Bring your village across

On the old website, open Settings and export your village JSON. Import it on this website. Saves are stored locally in your browser and do not move automatically between website addresses. No personal saves or GPS data are included in this repository.

## Development

Use Flutter stable with Dart 3.10 or newer. Run `flutter pub get`, `flutter test`, and `flutter run -d chrome`. The archive includes detailed gameplay documentation.
