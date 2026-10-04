# Omnarr: Home Assistant add-on

[Omnarr](https://github.com/tamengual/omnarr) puts the media apps you already run behind
one search and one library: Calibre, Audiobookshelf, Storyteller, Komga, Jellyfin, Sonarr,
Radarr, Seerr, Prowlarr, Shelfmark, RomM, ROMarr and Stash. It runs as a Home Assistant
add-on with its own sidebar panel.

## Install

1. In Home Assistant, go to **Settings → Add-ons → Add-on store → ⋮ → Repositories**.
2. Add `https://github.com/tamengual/omnarr-ha`.
3. Find **Omnarr** in the store, then click **Install**, then **Start**.
4. Open **Omnarr** from the sidebar and connect your apps in **Settings → Connections**.

Works on `amd64` and `aarch64` (Raspberry Pi 4/5, Home Assistant Green and Yellow, most
x86 boxes). This needs Home Assistant OS or Supervised. On Home Assistant Container or
Core, run the [Docker image](https://github.com/tamengual/omnarr#install-docker) instead.

See [the add-on docs](omnarr/DOCS.md) for addresses, database-file apps and direct access.

## Licence

GPL-3.0-or-later, the same as Omnarr.
