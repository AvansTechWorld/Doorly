# Doorly: a simple logger

Two things only:

- **Event attendance**: log who came to an event.
- **Area in / out**: log who goes into and out of an area (first entry = in, next = out).

Runs in any browser, works offline, keeps everything on the device. No server, no accounts.

## Set up
1. Put the folder on a web host (GitHub Pages works: push to `main`) or open `index.html` directly.
2. Open it once online, then install it from the browser menu so it works offline.
3. **Setup** tab: add your events and areas. Optionally add or import people (`id,name,group`).

## Use
- **Log:** pick *Event attendance* or *Area in / out*, choose the event or area, then type an ID or name and press Enter. A USB scanner works, and Android Chrome has a camera scan button (needs HTTPS).
- **Now:** who is inside each area right now (check people out one by one or all at once), and who attended today's events.
- **Records:** every entry, filter by date, event/area or name. Download as CSV. Delete a wrong entry.
- **Without a people list**, whatever is typed is logged as the name.

## Backups
Each device keeps its own data. Download a backup in **Setup**. To combine devices, use *Add another device's backup*. Clearing browser data deletes records.

## Updating
Replace the files and bump the version in `sw.js` (for example `doorly-v15`).

## Files
`index.html` the app · `config.js` optional starting events/areas · `sw.js` offline support · `manifest.webmanifest`, `icon-*` the installed look.
