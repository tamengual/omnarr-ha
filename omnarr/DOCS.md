# Omnarr

Omnarr puts the media apps you already run behind one search and one library: Calibre,
Audiobookshelf, Storyteller, Komga, Jellyfin, Sonarr, Radarr, Seerr, Prowlarr, Shelfmark,
RomM, ROMarr and Stash. Every app is optional.

## Getting started

1. Install and start the add-on, then open **Omnarr** from the sidebar. You're signed in
   through Home Assistant, so there's no separate password to create.
2. Omnarr opens on **Settings → Connections**. For each app you use, enter its address and
   API key, then press **Test**. Each card says where the app keeps its key.
3. Omnarr builds its search index (about a minute) and keeps it up to date every 15 minutes.

### Addresses

Enter the address *Omnarr* uses to reach each app:

- **Apps on another machine:** use that machine's address, e.g. `http://192.168.1.20:8989`.
- **Apps running as Home Assistant add-ons:** use the add-on's hostname, shown on its
  info page, with the app's port, e.g. `http://a0d7b954-sonarr:8989`.

## Apps that connect through a database file

Calibre, Storyteller and BookBridge have no usable API, so Omnarr reads their database file
read-only. That only works when the file is on this Home Assistant machine:

| Where the library is | Path to use in Omnarr |
|---|---|
| Home Assistant's media folder | `/media/...` |
| Home Assistant's share folder | `/share/...` |
| Another add-on's config folder | `/addon_configs/<addon>/...` |

If those apps run on a different machine, use the plain Docker image there instead; the
README explains how. All the API-based apps work from anywhere.

## Direct access (optional)

Opening Omnarr through the Home Assistant app or sidebar works everywhere, phones included.
If you also want a direct address, set a host port for `8765/tcp` in the add-on's
**Network** settings. Direct visitors sign in with Omnarr's own password, which you choose
the first time you open that address.

## Your data

The index, settings and API keys live in the add-on's private storage. Home Assistant
backups include them.
