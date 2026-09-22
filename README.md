# MVP × Midnite — Partnership Document

Single self-contained page. Two tabs:

- **Audience Demographics** — audience overview, broadcast and social distribution
- **Commercials** — heads of terms, framework and full asset schedule

## Deploying

Everything is in `index.html`; both logos are embedded, so there are no asset
paths to break. Put the file in the repo root and enable GitHub Pages
(Settings → Pages → Deploy from branch → root).

## Editing the live page

1. Open the hosted page.
2. Click any text and edit it. Changes save to your browser as you type.
3. Click **Download HTML**. You get an `index.html` with your edits written
   into the markup.
4. Commit that file over the existing `index.html`. The hosted page is now
   updated for everyone.

Step 3 is what makes the edit permanent — until then it only exists in your
own browser. **Reset** discards local edits and restores whatever the hosted
file says.

The downloaded file always opens on the first tab, and carries a fresh build
stamp so anyone's older saved edits are discarded rather than masking the
version you just published.

**Download PDF** opens the print dialog — choose "Save as PDF". A4 portrait,
both tabs, demographics first.

## Rebuilding

`make_tabbed_doc.py` regenerates this file. Commercials content is extracted
from the terms sheet rather than retyped, so the two cannot drift. The build
syntax-checks the emitted JavaScript with `node --check`.
