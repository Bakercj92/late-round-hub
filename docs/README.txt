late-round-tracker / dist
=========================

This folder is the hub. Open index.html (the front door: pick a league), or
bookmark a page directly.

WHAT UPDATES AND WHAT DOES NOT
  manifest.js + *.main.<hash>.js + *.text.<hash>.js   rewritten every build
  *.html shells + *.portal.html + index.html           only when the UI changes

So a normal update rewrites the data files and leaves the pages alone. You
refresh the page. There is nothing to import and no file to drag anywhere.

KEEP THE FOLDER TOGETHER
A shell holds no data. Moving one page somewhere else on its own gives you a
page that cannot load. Copy the whole folder or none of it.

IF SOMETHING IS WRONG
The header of every page shows the build stamp. If it is not moving, the build
is not running -- the page is doing its job.

For a board that depends on nothing at all, open tracker-artifact.html from the
parent folder. It is the same page with the data baked in, needs no network and
no sibling files, and is the draft-table fallback.
