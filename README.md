# Invoice Preflight — PDF invoice review pilot

Turn a folder of supplier invoice PDFs into a reviewable CSV and HTML report. The local Python prototype extracts invoice fields and highlights missing values, duplicate supplier/invoice-number pairs, and subtotal + tax vs. total mismatches. A person reviews the originals before any accounting use.

## What the current prototype demonstrates

- Runs locally without sending invoice data to a hosted service or creating accounting entries.
- Writes `invoices.csv`, `review.csv` and `review.html`.
- Handles simple labeled English and Bulgarian text PDFs, including Bulgarian invoice dates, BGN and decimal-comma amounts.
- Includes five **fictional** example PDFs: three English examples and two Bulgarian examples. The latter demonstrate a correct total and an incorrect total flagged for review.
- Six automated tests pass. This is a demonstration, not a measured production accuracy claim.
- Optional English OCR needs local Tesseract and always requires manual review. Bulgarian scanned PDFs need additional OCR work.

## €500 fixed-scope pilot

For €500, I will adapt extraction and checks to **5–10 representative, synthetic or appropriately redacted invoice templates** supplied by the buyer. The agreed delivery includes configured Python source, CSV/HTML review output, instructions and one correction round for those layouts. We will agree on fields and acceptance examples before starting. Suitable for a small finance or operations team reviewing supplier bills by hand.

The pilot does **not** include a QuickBooks API connection, automatic ledger posting, tax advice, unlimited formats, Bulgarian scanned-PDF OCR or guaranteed OCR accuracy. Additional work needs separate scope and testing.

**Interested?** [Contact me on LinkedIn](https://www.linkedin.com/in/dobromir-kostov-a04714262) with the subject “Invoice Preflight pilot” and the number of invoice layouts you need reviewed. Please share only synthetic or redacted samples initially.

The working source and example PDFs can be shared privately as part of a qualified pilot discussion. This public repository is a product overview, not a software download.
