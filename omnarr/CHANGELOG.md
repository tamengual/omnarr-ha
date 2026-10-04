# Changelog

## 0.3.0

- Accounts for everyone in your household. Each Home Assistant user gets their own Omnarr
  account automatically, and the first one becomes admin.
- Permissions per person: request downloads, save files to their device, upload, private section.
- Invitation links (copy, or email them), per-person progress, Save to device and uploads.
- `/share` is now mapped read-write so you can point uploads at a folder there. Omnarr
  only writes to the upload folders you set.

## 0.2.5

- Requested comics are fetched as comic archives and Komga is asked to rescan when they arrive.

## 0.2.4

- Request related books and comics in one click; Omnarr keeps looking until a good copy arrives.

## 0.2.3

- More accurate related-works matching (shows and movies match your library by id), and book lookups also try the subtitle.

## 0.2.2

- Related works for shows, movies, books and comics: the whole franchise, adaptations and source material, grouped and matched to your library.

## 0.2.1

- Built-in starter lists of well-known book→screen adaptations and shared universes (Middle-earth, the Cosmere, Dune…).
- Tested on a real Home Assistant OS install.

## 0.2.0

- First release as a Home Assistant add-on. Omnarr opens from the sidebar, and you're signed in through Home Assistant.
- Direct access on port 8765 is optional and uses Omnarr's own password. That password can only be set from inside Home Assistant, so nobody else can claim it first.
- Read-only access to `/media`, `/share` and other add-ons' config folders, for Calibre, Storyteller and BookBridge libraries kept on this machine.

Full app changelog: https://github.com/tamengual/omnarr/blob/main/CHANGELOG.md
