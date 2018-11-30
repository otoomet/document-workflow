# document-workflow

Code for creating an efficient parallel workflow for converting and OCR-ing a large number of text document to text

## Data files

The original lawsuit scanned pdfs are downloaded by the download
scripts into the
folder
`<DATADIR>/CaseFiles`.  The individual lawsuits are spread in the
folder structure as
`<DATADIR>/CaseFiles/State/<county>/<year>/<casenr>/`, and all the
original scans for a particular lawsuit are in this folder.

Both the OCR and address extraction scripts assume the files are layd
out like this.  It also permits a
special county, `Test`, to be located among counties.  Everything in
the Test county folder is ignored by the ocr script.

The OCR script mirrors the same structure for the ocr-d texts in
folders like
`<DATADIR>/txt/State/County/year/casenr/`.
