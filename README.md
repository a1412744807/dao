# DAO

A collection of HTML-based presentation tools and summary exporters designed to transform structured content into visually appealing digital assets (PNG images, ZIP archives, or PDFs).

## 🚀 Features

The repository contains several specialized HTML tools:

- **Card Exporters**: Converts HTML layouts into high-quality image cards (PNG). These are specifically styled for social media or slide-like presentations.
- **Bulk Export**: Integration with `JSZip` to bundle multiple generated images into a single downloadable ZIP file.
- **Summary Exporter**: A clean, document-style layout designed for monthly discussion summaries with a built-in "Export to PDF" feature using browser print styles.
- **Professional Styling**: Utilizes modern CSS, including Google Fonts (Noto Sans SC), gradients, and responsive layouts.

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Libraries**:
  - [html-to-image](https://github.com/bubkoo/html-to-image): For rendering HTML elements as PNG images.
  - [JSZip](https://stuk.github.io/jszip/): For client-side ZIP file creation.
  - [Lucide Icons](https://lucide.dev/): For clean, consistent iconography.

## 📖 Usage

Since these are standalone HTML files, no complex installation is required.

### Running the Project
1. Clone the repository to your local machine.
2. Open any of the `.html` files in a modern web browser (Chrome, Edge, or Firefox are recommended).
3. Interact with the UI to trigger exports:
   - **Single Export**: Click the "导出此卡片" (Export this card) button under a specific item.
   - **Bulk Export**: Click the "一键导出全部卡片为 ZIP" (Export all cards to ZIP) button at the top of the page.
   - **PDF Export**: In the summary documents, click the "导出为PDF" (Export to PDF) button to open the print dialog.

## 📝 Implementation Notes

- **Image Quality**: The exporters use a `pixelRatio` (typically 1 or 2) to ensure that the output images are crisp and suitable for high-resolution displays.
- **CORS & Fonts**: Some custom fonts are loaded via Google Fonts. If fonts do not appear in exported images, ensure you are running the file in an environment that allows cross-origin resource loading.
- **Print Optimization**: The summary files use `@media print` CSS rules to remove UI buttons and adjust margins automatically when exporting to PDF.
