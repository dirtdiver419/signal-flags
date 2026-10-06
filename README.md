# Signal flags

Three tabs:

- **Type**: spell a message in flags and read each flag's single-flag meaning. Optional realistic hoist with substitutes.
- **Flags**: tap flags (including substitutes and the answering pennant) to copy a hoist you can see, and read it flag by flag or as a Pub. 102 code group.
- **Dictionary**: search, or browse by section and subject, the general and medical signal code, the naval appendix, the icebreaker table, the complement and medical tables, and Chapter 4. Source chips (General, Medical, Appendix, Single flags, Procedure, Tables, Icebreaker, Chapter 4) narrow a search. Sections start collapsed. Footnote marks open their text on tap. Cross-references are links that jump to the target.

International Code of Signals or US Navy mode. Three looks: chart room, bridge, and plain.

Everything runs in the browser from one file. Nothing is saved or sent anywhere; the message,
mode, and look live only in the link. The source filter chips are not in the link.

Printing works from the browser's print command. A hoist on the Flags tab, or whatever Dictionary sections are open, prints on plain white with the controls hidden. Screen looks are unchanged.

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

- Signal text is taken from Pub. 102, International Code of Signals (NGA, 1969 edition revised 2020), a U.S. government work with no copyright claimed. Spellings and punctuation are as printed in the 2020 edition, including its typos.
- Signals included: 1,875 in all. General code 1,374 (648 main signals and 726 complements), medical code 445, and the appendix 56 (52 U.S./Russia naval signals plus the four Russian warning signals SNG, SNO, SNP, SNR).
- Also included, as text: single-letter signals and single letters with numerals, the flag procedure signals, the icebreaker signals, Complements Tables 1 to 3 and the inline complement lists (JF, JP, JQ, UV 9, WY, XE), Medical Tables M-1 to M-3, and Chapter 4: distress signals, lifesaving Tables I to VI, medical transport identification, radiotelephone procedures, and radiotelephone Tables 1 to 3 (Table 1 is the radiotelephone phonetic alphabet and figure spelling).
- Not included: Morse tables, the phonetic tables in Chapter 1, the Chapter 1 section 6 to 9 procedure text, the lifesaving pictograms (Chapter 4 Section 2 is text only), the Chapter 3 explanation and instruction text, Figures 1 and 2, and semaphore, flashing light, and sound procedures. The substitute rules are built into the app but their Chapter 1 text is not shown.
- Titles for the complement tables and Tables M-1 to M-3 are labels written for this page. The data carries no title for them.
- Twenty-eight general codes and 122 medical codes are absent from the book itself and so from this app. "CD 9" is signal CD with complement 9. The appendix mark on "NAVAL VESSELS*" has no footnote text in the source. Three contents page numbers are off by one in the source.
- One display change: a Chapter 4 distress line reaches the data with the PDF glyph code for the Morse dots, and the page draws them as bullets. The data is unchanged.
- Navy single-flag meanings come from publicly circulated sources and are not official. Pub. 102 has no Navy single-flag table; only the U.S./Russia appendix is official Navy content in it. Many letters have no public single-flag meaning, and those stay blank on purpose.
- Flag artwork is drawn in code from the standard designs. Navy numeral 6, Navy numeral 0, and the
  4th substitute were checked against fewer sources than the rest.
