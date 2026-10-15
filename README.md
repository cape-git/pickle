# Pickleball Tournament app

Upload everything in this folder (keep the `icons` and `lib` folders) to any HTTPS static host,
for example GitHub Pages or GitLab Pages. Then open the page on your phone and:

- **iPhone (Safari):** Share button → *Add to Home Screen*
- **Android (Chrome):** menu → *Install app* (or *Add to Home screen*)

All data (members, locked teams, the running tournament) is stored on the device.
Use *Settings → Export members* to keep a copy of the member list.

## Sharing the member list

A new install starts with an empty member list.

1. Add the members on your own phone: *Settings → Club members*.
2. *Settings → Export members* saves `pickleball-members-<date>.json` (names only). Send that file along with the link.
3. Each person opens the link, installs the app, saves the file on their phone,
   and taps *Settings → Import members* to load it.

Importing replaces the member list on that phone. Rounds, results and settings are not touched.

## Updating

When you change `index.html`, also change `VERSION` in `sw.js` (e.g. `pickleball-v10`)
so installed copies pick up the new version.
