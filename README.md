# Papers

LaTeX monograph and study-note repository focused on React UI systems, component-library architecture, and related technical writing.

## Layout

- `uilibraries.tex`: main manuscript entry point.
- `ui_code_reference_library.tex`: include hub for the modular manuscript sections.
- `sections/`: manuscript modules, appendices, and reference chapters.
- `notes/`: smaller companion study notes.
- `scripts/`: helper scripts used during manuscript cleanup and recovery.
- `archive/`: backups and generated artifacts kept out of the active source root.
- `references.bib`: bibliography for the manuscript.

## Build

Run the manuscript from the repository root:

```bash
pdflatex -interaction=nonstopmode -halt-on-error uilibraries.tex
pdflatex -interaction=nonstopmode -halt-on-error uilibraries.tex
```

The first pass builds the document and the second pass settles references, TOC entries, and outlines.

## Notes

- Build outputs are not meant to live in the active root. They are archived under `archive/generated/` during cleanup work.
- Legacy backups are kept under `archive/backups/`.
- The repository keeps modular LaTeX sources split by topic so the manuscript can grow without turning the root into a flat dump of files.
