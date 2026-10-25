# PO Auto Entry

**Offline PDF Purchase Order OCR to Excel — Proof of Concept v0.1**

PO Auto Entry is an experimental Windows desktop application that explores extracting purchase order information from PDF documents and exporting structured data to Excel.

The project focuses on an offline OCR workflow with human verification before exporting results.

## Features

- Offline OCR using Tesseract
- Batch PDF processing
- Custom OCR region selection
- Order Code, Description, Quantity and Price extraction
- Manual review with keyboard shortcuts
- Duplicate and incomplete record handling
- Export to a new Excel file or a compatible existing template
- Selectable Excel export destination
- Windows desktop interface

## Workflow

1. Select a folder containing purchase order PDFs.
2. Configure OCR regions for the document layout.
3. Run batch OCR.
4. Review extracted information against the original PDF.
5. Correct errors and resolve exceptions.
6. Confirm verified records.
7. Export the results to Excel.

## Testing

The prototype has been tested with three synthetic PDF datasets:

| Dataset | Documents | Layout |
|---|---:|---|
| Batch A | 15 | Standard |
| Batch B | 30 | Compact |
| Batch C | 50 | Form Style |
| **Total** | **95** | **3 layouts** |

All three batches completed preliminary workflow and Excel export testing.

These results do not establish production readiness or OCR accuracy on real-world documents.

## Known Limitations

- Multi-line purchase order item extraction is not supported.
- OCR may fail or produce incorrect values.
- Handwritten and low-quality documents may require extensive manual correction.
- Custom Excel template creation and design within the application are not supported.
- OCR regions must be configured for different document layouts.
- Source Page information may be missing.
- Manual verification is required before exporting.
- This prototype is not intended for production or business-critical use.

## Download

Download the Windows prototype from the GitHub Releases section.

The application is intended to run locally. Please review the release notes and system requirements before testing.

## Development

This project was developed with extensive AI-assisted coding, focusing on workflow design, testing and experimentation.

## Feedback

Bug reports, suggestions and feature requests are welcome through GitHub Issues.

## Roadmap

- OCR diagnostics and performance improvements
- Adaptive OCR and additional offline OCR engines
- Multi-line item extraction
- Improved document layout support
- Custom Excel template configuration

## Disclaimer

This software is an experimental proof of concept. Always verify extracted data before use. Do not rely on it for business-critical processing.

