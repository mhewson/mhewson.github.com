# Pile of Shame Slayer 🎲

A free, single-file web app for miniature painters with a big backlog.
Add your unpainted units, roll a random project, a colour-scheme card and a
technique, then log what you paint and watch the pile shrink.

**Live app:** https://mhewson.github.io/

<!-- Add a screenshot here: ![Screenshot](screenshot.png) -->

## Why

Sitting down with a huge backlog and no idea where to start is a good way to
paint nothing. This tool picks for you, keeps track of what you've done, and
makes small wins visible.

## Features

- **Roll a session**: a random project, a card number from the Deck of Many
  Colors (fantasy deck, sci-fi deck, or both, cards 1 to 50) and a technique
  such as speed paint, NMM, airbrush skill builder, filters, desaturate,
  saturate, underpaint or texture. Lock any part and reroll the rest.
- **Recipes**: once you've painted one mini with a rolled card and technique,
  make it the recipe for the rest of that entry, or for every entry in the same
  project, so the whole unit matches.
- **Collection tracking**: minis done, total and % complete for each entry,
  with manufacturer, material (plastic, metal, resin), project tags and
  purchase date.
- **Dates**: time from purchase to first mini painted, and to finished.
- **Effort labels and badges**: fun labels for how many minis you finish in a
  sitting, plus milestone badges and a day streak.
- **Painted gallery**: log what you painted with a description, a photo and the
  paints you used, so you know what to pick out next time.
- **Search, filters and pages**: filter by project, manufacturer, material and
  status. The roll can stay inside your filters, for example "only this
  project".
- **Challenge mode**: set a deadline, commit entries, take a dated before photo
  and after photo, and get a pace check and a summary to share. Inspired by
  [Miniac's The Finisher](https://www.youtube.com/watch?v=a6L4wNoaHoM).
- **Undo**: every log has an undo, and each entry has a minus button.
- **Import and backup**: paste or upload a spreadsheet, and copy a full
  backup you can restore later.

## Using it

Open the live link, or keep your own copy. There is nothing to install.

### Get your own copy

It is one file, so copying it is easy, and the MIT licence lets you keep,
change and share it.

- **In the app:** scroll to **Share this app** and press **Save a copy of this
  app**. That gives you a single file to keep or send to a friend, who just
  double-clicks it. No GitHub account needed.
- **Download it:** open [`index.html`](index.html) in this repository and click
  the **Download raw file** button, or use **Code → Download ZIP**. Save it
  anywhere and double-click it to open it in your browser.
- **Make your own version:** click **Fork** at the top of this page. In your
  fork go to **Settings → Pages**, choose **Deploy from a branch**, pick
  `main` and `/ (root)`, and you will have your own live link to change as you
  like.

Your painting data is saved in your browser for whichever address or file you
open, so a downloaded copy starts with an empty pile. To move your pile between
copies, use **Copy full backup** and paste it into the import box of the other
one.

### Importing from a spreadsheet

Paste cells or upload a CSV in the import box. Columns, in this order:

| Name | Total minis | Done (optional) | Manufacturer | Material | Date bought | Projects |
|------|-------------|-----------------|--------------|----------|-------------|----------|
| Ork Boyz | 10 | 3 | Games Workshop | Plastic | 2024-01-15 | Waaagh;Ork army |

A header row is fine. Separate several projects with `;`. Material is
Plastic, Metal or Resin. Dates use YYYY-MM-DD.

### Backup and restore

Your data is saved **only in your own browser, on your own device**. Nothing is
sent anywhere. Clearing your browser data will erase it, so use **Backup** at
the bottom of the page:

- **Copy full backup** copies everything (including photos and history). To
  restore, paste it into the import box and press Import.
- **Copy as spreadsheet (CSV)** copies your entries in the import format above.

## Tech

One HTML file with plain JavaScript and CSS. No framework, no build step, no
dependencies, no network requests. Data is stored in `localStorage`.

## Ideas

- Shared hub for painting groups, with a paint-along mode
- Session timer and short-session tasks
- Per-entry paint stages (primed, based, shaded, highlighted)
- "Done by" targets for individual sets

## Credits and disclaimer

Inspired by [Ninjon's Deck of Many Colors](https://www.youtube.com/watch?v=Qc9zaP75He8&t=936s), [Miniac's The Finisher](https://www.youtube.com/watch?v=a6L4wNoaHoM) and the
videos of [Amalia's Miniatures](https://www.youtube.com/@Amaliasminiatures).
This is an independent hobby project and is not affiliated with or endorsed by
any of them, nor by any miniature manufacturer. Product names used in examples
belong to their owners.

## Licence

MIT. See [LICENSE](LICENSE).
