<h1 align="center">Protein Sequence Formatter</h1> <h3 align="center">Format • Preview • Export DOCX — all client‑side</h3><p align="center"> <a href="./LICENSE"> <img src="https://img.shields.io/badge/License-MIT-yellow.svg"> </a> <a href="https://cdnjs.com/libraries/docx"> <img src="https://img.shields.io/badge/docx-7.8.0-5C6BC0?logo=microsoftword&logoColor=white"> </a> <img src="https://img.shields.io/badge/Built%20with-Vanilla%20JS-F7DF1E?logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/Status-Stable-brightgreen"> </p>

 <b>Overview</b>

Paste a protein sequence, choose a layout, preview instantly, and generate a compact DOCX file. Runs entirely in your browser—no backend, no build step.

 <b>Features</b>

Input validation with auto-clean (keeps A–Z; strips others; uppercases)
Live residue count and real-time preview
One-click DOCX export via docx
Responsive, clean UI

 <b>Supported Formats</b>

Continuous — 10 residues/line with positions
Compact Grid — 20 residues per row, spaced
FASTA-style — 60 chars/line with auto header
Multi-column Table — 4 columns of Pos/Res

 <b>Quick Start</b>

Download/clone this repo
Open index.html in a modern browser
Paste sequence → select format → click “Generate DOCX File”

 <b>Tech Stack</b>

HTML CSS JavaScript docx@7.8.0

 <b>Customization</b>

Lines/rows: edit chunk sizes in formatSequence() (10/20/60)
Table columns: change const cols = 4
Filename: tweak link.download in generateDocx()
Fonts/sizes: adjust TextRun({ font, size })

 <b>Privacy</b>

100% client-side; data never leaves your browser.

 <b>Troubleshooting</b>

Generate button disabled → ensure at least one A–Z letter is present
“Non-amino acid characters removed” → cleaner stripped invalid chars/whitespace
CDN blocked/offline → download docx.min.js locally and update the script tag

 <b>License</b>
MIT — see LICENSE.
<b>Acknowledgements</b>

DOCX generation powered by the excellent <a href="https://github.com/dolanmiu/docx">docx</a> library.

##  Access Here - https://protein-sequence.netlify.app

<b>Preview</b>
<img width="663" height="950" alt="brave_screenshot" src="https://github.com/user-attachments/assets/03c99045-5df2-4ec1-bdd3-fdc0a9b1634b" />
