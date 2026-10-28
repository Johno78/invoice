# Invoice Reader

A single-page tool for reading supplier invoice PDFs and copying the figures into accounts software.

Drop one or more text-based invoice PDFs onto the page. For each one it pulls out the supplier, invoice number, date, PO number, net, VAT and total, checks that net + VAT = total, and gives you a copy button next to each figure. You can paste a list of open purchase orders to check each invoice against its PO.

- Runs entirely in the browser. PDFs are read locally and are never uploaded.
- Text-based PDFs only. Scanned or photographed invoices need OCR, which is not included.
- Always compare the figures with the PDF before posting anything.
- Nothing is posted to Sage or any other system. It only reads and helps you copy.

## Use it

Open the page, then drop PDFs on it or use Choose PDFs. If dragging an attachment straight from an email program does nothing, save the PDF first and drop it from your Downloads or desktop.

## Notes

- Uses [pdf.js](https://mozilla.github.io/pdf.js/) (loaded from cdnjs).
- Remembers which invoices you have ticked as entered, supplier name corrections and your pasted PO list in the browser's local storage on that device only.
- Everything is in `index.html`.
