## LaTeX Version of DFG Project template 53_01_en_elan.rtf

This is a LaTeX version of the [DFG](https://www.dfg.de) template for
project proposals within the [SPP 2458 Combinatorial
Synergies](https://combinatorial-synergies.de) created by [Thomas
Kahle](https://www.thomas-kahle.de).  It comes **with no warranty or
responsibility whatsoever**.  When in doubt about proposal formatting
or requirements, always consult with the DFG.

**Updated 2026-04-21** to match the current DFG templates
(`53-01-en-elan` version 09/25, `53-200-en-elan` version 07/25).

- [Official Documentation on the DFG homepage](https://www.dfg.de/foerderung/programme/koordinierte_programme/schwerpunktprogramme/formulare_merkblaetter/index.jsp)

- The DFG suggests Arial font which is unavailable in standard LaTeX.
  If you want to stay close to that suggestions, uncomment lines 8 and
  9 in the .tex to activate Helvetica.

- The font size should be at least 11pt with 1.2 line spacing.  This
  should be satisfied with LaTeX's 11pt setting.  For the references
  a minimum font size of 9pt is required.
  
- The finished proposal has a page limit of 17 pages for Sections 1-3
  and an additional 8 pages for the remaining sections.  Proposals are submitted
  through [elan](https://elan.dfg.de)

- There are many sections which are not relevant to all proposals.
  For example Clinician Substitutes cannot be applied for within a
  math project.  Mercator fellows, workshops and Gender equality
  measures are all centrally applied for within an SPP.  Consequently
  these can be removed.  The template stays close to the original rtf.
  
- The proposal uses `biblatex` with the `biber` backend (not BibTeX).
  Build with `pdflatex template.tex`, then `biber template`, then
  `pdflatex template.tex` twice.  Include the keyword `vorarbeit` in
  your max. 10 publications to be highlighted in the bibliography.

- Only the project description template (`53.01`) is implemented in
  LaTeX.  A separate CV template (`53.200`) must be submitted alongside
  the proposal; the current RTF is included here for reference.  
  Per DFG instructions, the CV must not exceed
  four pages, use at least Arial 11pt with 1.2 line spacing, contain
  no photograph, and be named `CV_PubList_<lastname>`.

## License

The LaTeX template and other original content in this repository are
published under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html.en).

The DFG RTF templates (`53_01_en_elan_*.rtf`, `53_200_en_elan_*.rtf`)
are **not** covered by the GPL.  They are cited here as distributed
on the [DFG homepage](https://www.dfg.de) and are provided as-is for
reference.
