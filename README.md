# Invoice Preflight — PDF invoice review pilot

Turn a folder of supplier invoice PDFs into a reviewable CSV and HTML report. The local Python prototype extracts invoice fields and highlights missing values, repeated supplier/invoice-number pairs, and subtotal + tax vs. total mismatches. Scanned PDFs can use local Tesseract OCR when installed. A person should review flagged items before accounting use.

## What the current prototype demonstrates

- Runs locally on PDFs without sending invoice data to a hosted service.
- Writes invoices.csv, review.csv and review.html.
- Includes three **fictional** invoice PDFs: one passes the automated checks, two are flagged for review (a total mismatch and a repeated invoice number).
- Five automated tests pass on the prototype. This is a demonstration, not a measured production accuracy claim.

## €500 fixed-scope pilot

For €500, I will adapt the extractor and checks to **5–10 representative, redacted invoice templates** provided by the buyer, then deliver the configured Python source, CSV/HTML review output, and setup notes. We will agree on the sample templates and acceptance examples before starting. Suitable for a small finance or operations team that currently reviews PDF supplier bills by hand.

The pilot does **not** include a QuickBooks API connection, automatic ledger posting, tax advice, unlimited invoice formats, or guaranteed OCR accuracy. Those would require separate scope and testing.

**Interested?** [Contact me on LinkedIn](https://www.linkedin.com/in/dobromir-kostov-a04714262) with the subject “Invoice Preflight pilot” and the number of invoice layouts you need reviewed. Please redact customer and payment details before sharing samples.

The working source and example PDFs are shared privately as part of a qualified pilot discussion. This public repository is a product overview, not a software download.
