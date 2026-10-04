# Signal flags

Type a message, see it as maritime signal flags, and read what each flag means on its own.
International Code of Signals or (unofficial) US Navy meanings, with an optional realistic
hoist that uses substitute pennants. Three looks: chart room, bridge, and plain.

Everything runs in the browser from one file. Nothing is saved or sent anywhere; the message,
mode, and look live only in the link.

## Files

- `index.html` is the whole app.
- `.nojekyll` tells GitHub Pages to serve the files as-is instead of running them through Jekyll.
- `README.md` is this file. GitHub Pages ignores it when serving the site.

## Put it on GitHub Pages

1. Create a new repository on GitHub (for example `signal-flags`).
2. Upload the **contents** of this folder, not the folder itself, so `index.html` sits at the top level of the repo.
   `.nojekyll` is a hidden file, so if your file picker hides it, drag the files in from a file manager that shows hidden files, or create an empty file named `.nojekyll` in the repo with "Add file > Create new file".
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, then Save.
5. Wait a minute or two. The site appears at `https://<your-username>.github.io/signal-flags/`.

To update later, upload the new `index.html` over the old one. Pages redeploys on its own.

## Keeping it out of search engines

`index.html` carries `noindex` robots tags, which tell Google, Bing, and other well-behaved
crawlers not to list the page. That only works if crawlers are allowed to read the page, so
there is deliberately no `robots.txt` blocking it. (A `robots.txt` inside a project repo would
be ignored anyway, since crawlers only check the root of `<username>.github.io`.)

Limits worth knowing:

- `noindex` keeps the page out of search results. It does not make it private. Anyone with the link can open it.
- If the repository is public, the source code is public too, even though the site isn't indexed.
- Crawlers that ignore the rules can still read the page. There's nothing personal on it to find.

## Notes

- ICS meanings are paraphrased from Pub. 102, International Code of Signals.
- Navy meanings come from publicly circulated sources and are not official. Many letters have no
  public single-flag meaning, and those stay blank on purpose.
- Flag artwork is drawn in code from the standard designs. Navy numeral 6, Navy numeral 0, and the
  4th substitute were checked against fewer sources than the rest.
