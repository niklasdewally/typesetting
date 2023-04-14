# Typesetting 

My personal config for typesetting / writing reports, notes, etc.

Primarily, this uses *pandoc* to export to pdf via *LaTeX*, but sometimes *HTML*
output is useful too.


## Report

The `report` folder contains all the boilerplate (Makefile, citation style,
etc) I use to write a coursework report.

To write a report using this, I copy this folder, and edit `report.md` and
`references.bib`

- The `preamble.tex` file defines common preamble / header that I use to
  customise the look of my document. This includes modifying margins, fonts, as
  well as force figures to appear in the place they are in the report.

* Pandoc settings are specified in `report.yaml`
