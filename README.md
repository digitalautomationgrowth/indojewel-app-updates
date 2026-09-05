# indojewel-app-updates

Update feed and remote kill-switch for the INDOJEWEL Invoice Processor.

**This repository must stay PRIVATE.** It carries the licence control file, and
the application reads it with a token that is compiled into the EXE.

| File | What it does |
|---|---|
| `version.txt` | `version\|download-url\|filename` — the app compares its own version against the first field and offers the update when this one is higher |
| `update_notes.txt` | the changelog shown inside the update dialog |
| `licenses.json` | remote kill-switch, keyed by Machine ID |

`version.txt` and the release asset are written by the License Manager's
**Publish Update** tab. Editing them by hand is possible but not the intended
route — publish from the manager so the release and the pointer to it are
always in step.
