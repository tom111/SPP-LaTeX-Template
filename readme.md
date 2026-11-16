## LaTeX Version of DFG Project template 53_01_en_elan.rtf

This is a LaTeX version of the [DFG](https://www.dfg.de) template for
project proposals within the [SPP 2458 Combinatorial
Synergies](https://combinatorial-synergies.de) created by [Thomas
Kahle](https://www.thomas-kahle.de).  It comes **with no warranty or
responsibility whatsoever**.  When in doubt about proposal formatting
or requirements, always consult with the DFG.

**Updated 2026-11-16** for the second funding period of SPP 2458.  It
matches the current DFG templates (`53-01-en-elan` version 09/26,
`53-200-en-elan` version 07/25) and the current Guidelines Priority
Programme (DFG form 50.05) and Proposal Preparation Instructions
(DFG form 54.01), both version 09/26.

- [Official forms and guidelines for Priority Programmes on the DFG homepage](https://www.dfg.de/en/research-funding/funding-opportunities/programmes/coordinated-programmes/priority-programmes/forms-guidelines)

### The 2026 call (second funding period)

- Call: [DFG Information for Researchers No. 50, 16 July
  2026](https://www.dfg.de/en/news/news-topics/announcements-proposals/2026/ifr-26-50).
  It invites proposals for the second three-year funding period.
- **Deadline: 30 November 2026.**  Proposals are submitted only via
  [elan](https://elan.dfg.de).
- First-time DFG applicants must **register in elan by 16 November
  2026** and select "SPP 2458" during the registration.
- Renewal of a project funded in the first period: in elan, use
  "Proposal Submission - Proposal Overview/Renewal Proposal" and select
  the funded project.  New project: use "Proposal Submission - New
  Project - Priority Programmes" and select "SPP 2458".
- Rules: DFG form 50.05, section B "Individual Projects within
  Existing Priority Programmes", and DFG form 54.01.
- Themes: enumeration, Dynkin classification, commutative algebra,
  matroids, convexity, lattice points, statistics, non-linear
  optimisation, mathematical physics.  Extremal and additive
  combinatorics are not central to the programme.
- The call strongly encourages proposals to outline how synergies
  between human mathematical insight and AI-supported methods
  (mathematical software, databases, machine learning, AI agents,
  formalisation, under the FAIR principles) advance their goals.
- The review panel meets online, without the applicants.
- Contacts: Prof. Dr. Christian Stump (Ruhr-Universität Bochum),
  coordinator of the SPP, for scientific questions.  Dr. Carsten
  Balleier, programme contact at the DFG Head Office.

### Formal requirements and the template

- Page limits: at most 17 pages for Sections 1-3 and at most 8 pages
  for Sections 4 and 5, 25 pages in total.  These limits are set by
  DFG form 54.01 and the 53.01 template.  The call sets no other
  limit.  As in the DFG form, Section 4 starts on a new page, and the
  running head counts the pages against the respective limit ("page 3
  of max. 17").
- Font at least Arial 11pt with line spacing at least 1.2, and at
  least Arial 9pt in the publication list.  The template sets the body
  text in LaTeX's 11pt size (10.95pt) on 13.26pt baselines, that is,
  1.21 times the font size, and the publication list in 10pt.  The
  stock `amsart` setting (13pt baselines, factor 1.19) fell slightly
  short, so `template.tex` now stretches it with `\linespread{1.02}`.
  The text area of the template is smaller than that of the DFG
  template, so a page holds about 15% less text than the Word template
  with Arial 11pt.
- Arial is unavailable in standard LaTeX.  For a similar look,
  uncomment the two Helvetica lines below the comment "DFG: font not
  smaller than Arial 11pt" in the preamble.
- The DFG asks applicants to keep the headings and numbering of the
  form.  Keep the headings of points that do not apply and write "Not
  applicable." there.  In SPP 2458, Mercator Fellows (5.5) and
  workshops (5.6) are requested by the coordination project, not by
  the individual projects (SPP website).  The standard allowance for
  equity and diversity (5.8) can only be requested in the
  coordination project.
- Renewal proposals report on the previous work in Section 1 and
  state in 2.1 since when the project has been running (DFG form
  54.01).  Preliminary work funded by the DFG should name its funding
  period.
- Section 2.2 should say which of the nine themes the project
  addresses and how it is integrated into the Priority Programme,
  including cooperation with other projects (DFG form 54.01, Special
  Instructions for Priority Programmes).  The template has comments
  with these points.
- If generative AI was used to prepare the proposal, the proposal must
  say which models were used, for what purpose and to what extent
  (DFG form 54.01).  The template has a note in 4.12.
- The DFG instructions (green) and comments (red) in the PDF are
  hidden by uncommenting `\renewcommand{\dfg}[1]{}` and
  `\renewcommand{\tk}[1]{}` in the preamble.
- In elan, name the PDF of the project description
  `Beschreibung_des_Vorhabens`.  PDFs must not exceed 10 MB and must
  allow reading, copying and printing.

### Bibliography

- The proposal uses `biblatex` with the `biber` backend (not BibTeX).
  Build with `latexmk -pdf template.tex`, or with `pdflatex template`,
  then `biber template`, then `pdflatex template` twice.
- The DFG asks for a DOI or URL where available.  The bibliography
  prints the DOI, otherwise the arXiv identifier (`eprint`), otherwise
  the URL.
- Include the keyword `vorarbeit` in your max. 10 publications to be
  highlighted in the bibliography.  LaTeX warns if more than ten
  entries carry it.  The limit holds for all applicants together.

### What changed in November 2026

The DFG template 53.01 version 09/26 differs from version 09/25 in
three points, all implemented:

- 4.1.1 is now "General ethical aspects and obligations" and ends with
  "A statement by an ethics committee is required: yes / no" (delete
  as applicable).
- The former 4.1.2 "Descriptions of proposed investigations on humans,
  human materials or identifiable data" was removed, so the remaining
  points of 4.1 moved up by one.
- Module 5.7 "Public Relations" is now "Science Communication".  A
  lump sum of up to EUR 1,000 per funding year and project can be
  requested with a short description of the activities (DFG form
  52.07).

The template also follows the form more closely than before: Section
1 is "Starting Point" with the subheading "State of the art and
preliminary work", "Risks in international cooperation" (4.1.4.2) and
the sustainability statement (4.1.5) sit inside 4.1 so that 4.2-4.12
carry the form's numbers, the items of 5.1.2 and 5.1.3 are numbered,
and the first page carries the form's title block instead of a
separate title page and table of contents.

### Curriculum vitae

Only the project description template (`53.01`) is implemented in
LaTeX.  A separate CV template (`53.200`, version 07/25, unchanged
since the April 2026 update) must be submitted alongside the proposal.
The current RTF is included here for reference.  Per DFG instructions,
the CV must not exceed four pages, use at least Arial 11pt with 1.2
line spacing, contain no photograph, and be named
`CV_PubList_<lastname>`.  Its list of scientific results has a
mandatory Category A (at most ten peer-reviewed publications) and an
optional Category B (at most ten other published results), each
numbered.

### DFG forms in this repository

- `53_01_en_elan_2026.rtf`: project description, version 09/26
  (current, implemented in `template.tex`).
- `53_01_en_elan_2025.rtf` and `53_01_en_elan_2023.rtf`: versions
  09/25 and 09/22.
- `53_200_en_elan_2025.rtf`: curriculum vitae, version 07/25
  (current).  `53_200_en_elan_2023.rtf`: version 03/23.

## License

The LaTeX template and other original content in this repository are
published under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html.en).

The DFG RTF templates (`53_01_en_elan_*.rtf`, `53_200_en_elan_*.rtf`)
are **not** covered by the GPL.  They are cited here as distributed
on the [DFG homepage](https://www.dfg.de) and are provided as-is for
reference.
