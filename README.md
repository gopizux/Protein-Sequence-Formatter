Protein Sequence Formatter
Format protein sequences and export compact, publication-ready DOCX files — all in your browser. No build step, no backend.
Features
🧪 Input validation with auto-cleaning (keeps A–Z, strips everything else)
🔢 Live residue counter
👀 Real-time preview
🗂️ Four output styles:
Continuous (10 residues/line, numbered)
Compact Grid (20 residues/row, spaced)
FASTA-style (60 chars/line with header)
Multi-column Table (Pos/Res in 4 columns)
📄 One-click DOCX export (via docx library)
📱 Responsive UI, works offline (if you bundle the library locally)
Quick Start
Clone or download this repository (single HTML file).
Open index.html in a modern browser.
Paste your protein sequence, choose a format, then click “Generate DOCX File”.
Note: The app uses a CDN for the docx library. You’ll need an internet connection unless you vend the library locally.

Usage
Paste your sequence into the textarea.
Allowed characters: A–Z letters
Whitespace/newlines are ignored
Input is uppercased automatically
Non-letters are removed (you’ll see a small notice)
Pick a format. The preview updates instantly.
Click “Generate DOCX File” to download:
Filename pattern: protein_sequence_{N}res_{format}.docx

How it Works
Vanilla HTML/CSS/JS with a single dependency: docx (CDN)

Core functions:
validateSequence() cleans input and updates state
getSequence() returns the compact sequence (A–Z only)
formatSequence(format, sequence) renders preview text
generateDocx() builds the DOCX (text or tables) and downloads it
Exports include a centered title: “Protein Sequence (N Residues)”
Monospace font (“Courier New”) is used for continuous/grid/FASTA output
Technology
Frontend: Vanilla JS, CSS, semantic HTML
DOCX generation: docx 7.8.0 via CDN
