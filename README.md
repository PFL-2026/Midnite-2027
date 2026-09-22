# MVP × Midnite — Partnership Document

Single self-contained page. Two tabs:

- **Commercials** — heads of terms, partnership framework and full asset schedule
- **Audience Demographics** — broadcast and social distribution

## Deploying

Everything is in `index.html`: both logos are embedded as base64, so there are
no asset paths to break. Drop the file in the repo root and enable GitHub Pages
(Settings → Pages → Deploy from branch → root). It also works opened directly
from disk.

## Using it

- Click any text to edit. Edits save to the browser and survive a refresh.
- **Reset** restores the original copy.
- **Download PDF** opens the print dialog — choose "Save as PDF". The PDF is A4
  portrait and contains **both** tabs, with the demographics starting on a new
  page.

Edits are stored per browser under the key `mvp-midnite-doc-v1`. They are not
committed back to the file — to make a change permanent, edit `index.html`.

## Rebuilding

`make_tabbed_doc.py` builds this file. The commercials content is extracted
from the terms sheet rather than retyped, so the two cannot drift apart.
