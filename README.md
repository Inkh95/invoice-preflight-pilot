# Invoice Preflight — offline PDF invoice review

Invoice Preflight reads selected supplier invoice PDFs locally and creates CSV and HTML reports for human review. It highlights missing fields, repeated invoice numbers, currency conflicts and subtotal + tax versus total mismatches. It does not post entries to accounting systems.

## Desktop beta (September 2026)

- A graphical interface lets users select PDF files, choose an output folder, run checks and open the report without a command line.
- Supports simple labeled English and Bulgarian text PDFs, Bulgarian dates, BGN and decimal-comma amounts. The sample invoices are fictional.
- Eleven automated tests pass, including missing and damaged file handling. These are not a measurement of accuracy on production invoices.
- A Windows executable was built in private GitHub Actions and the command-line version passed a Windows smoke test. The graphical application still needs an interactive check on a clean Windows computer.
- Optional offline OCR requires separately installed Tesseract and pdftoppm. English OCR has been tested; Bulgarian OCR configuration exists but has not been validated with scanned Bulgarian documents.
- Files remain on the user's computer. Original invoices must be verified before any accounting action.

**Status:** private technical beta, not yet an instant-download retail product. Realistic redacted formats, interactive Windows validation and secure post-payment delivery are needed before launch.

## €500 fixed-scope customization pilot

For €500, I can adapt extraction and checks to **5–10 agreed, appropriately redacted invoice templates** supplied by a buyer, with configured source, CSV/HTML output, setup notes and one correction round. Scope and acceptance examples must be agreed before work begins. QuickBooks integration, automatic posting, tax advice, unlimited formats and guaranteed OCR accuracy are outside this pilot.

**Interested in a demo or pilot?** [Contact me on LinkedIn](https://www.linkedin.com/in/dobromir-kostov-a04714262) with the subject “Invoice Preflight pilot”. Please share only synthetic or redacted samples initially.

The working source and example PDFs are held privately. This public repository is a project overview.
