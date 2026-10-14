# Adobe Acrobat Reader DC — Enterprise Web Application

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Status: Production Ready](https://img.shields.io/badge/Status-Production%20Ready-success.svg)
![PWA Offline Ready](https://img.shields.io/badge/PWA-Offline%20Ready-orange.svg)
![Zero Backend Required](https://img.shields.io/badge/Architecture-100%25%20Client--Side-brightgreen.svg)

A high-fidelity, client-side web replica of **Adobe Acrobat Reader DC Continuous Track**, engineered with full PDF document manipulation, annotations, interactive AcroForm designer, digital PKI certificate signing, preflight standards, CAD measurement, and a neural **Bangla OCR & Font Engine**.

---

## 🚀 One-Click Deploy to Vercel

You can deploy this application directly to **Vercel** with zero configuration:

1. Click the **Deploy with Vercel** button above or push this repository to GitHub.
2. In Vercel, import your Git repository.
3. Keep the default settings (`Framework Preset: Other`, Output Directory: `./`).
4. Click **Deploy**. Your Acrobat Reader web instance will be live globally in seconds!

---

## 🌟 Key Features

### 1. Document Viewing & Navigation
* Continuous multi-page scroll, single-page view, and read mode.
* Zoom engine (50% to 300%, Fit Width, Fit Page).
* Page thumbnails with live indicators and bookmark navigation rail.
* Fast full-text document search with highlighted match counters.

### 2. Fill & Sign Engine
* Interactive text box placement with font sizing (A+/A-) and typography switching.
* Native symbol stamps: Checkmark (✓), Crossmark (✗), Bullet (●), Line (—), Circle (◯).
* Signature creation: Canvas hand-drawn signature, type-to-sign, and transparent PNG image upload.
* Drag-and-drop repositioning directly on document canvas.

### 3. Annotation & Commenting Studio
* Text highlights, strikethroughs, squiggly underlines.
* Interactive sticky notes with collapsible review comment threads.
* Drawing tools: Freehand brush/pencil, line, rectangle, ellipse, and arrow.
* Stamp catalog: Approved, Confidential, Draft, Received, and custom stamps.

### 4. Bangla OCR & Font Library (বাংলা ইঞ্জিন)
* **Variable Bangla Fonts**: Bundled offline *Noto Sans Bengali* and *Noto Serif Bengali* with fallback to *Hind Siliguri* and *Kalpurush*.
* **OpenType Ligatures**: Flawless rendering of complex conjuncts (যুক্তবর্ণ যেমন ক্ষ, জ্ঞ, ঙ্ক, ণ্ড, ইত্যাদি) without tofu boxes or broken glyphs.
* **Dual OCR Modes**:
  * **Neural Visual OCR**: Tesseract.js engine powered by local offline `ben.traineddata.gz` for scanned photocopies, circulars, and image documents.
  * **Digital Text Stream Extraction**: Reconstitutes native text layers with layout and line-break preservation.
* **Bijoy to Unicode Converter**: 1-click conversion of legacy SutonnyMJ/Bijoy documents (`Avwg evsjvq Mvb MvB` ➔ `আমি বাংলায় গান গাই`).
* **Matra & Typo Fixer**: Corrects separated matras, ZWNJ sequences, and misplaced nuktas (ড়, ঢ়, য়).
* **Document Injection**: Directly inserts recognized text into the PDF via Fill & Sign.

### 5. Interactive Form Designer (AcroForms)
* Visual drag-and-drop form field builder:
  * Text Fields
  * Checkboxes
  * Radio Button Groups
  * Dropdown Selectors
  * Digital Signature Fields
* Compiles into true native PDF AcroForms compatible with desktop Adobe Acrobat.

### 6. Security, Legal & PKI Engine
* **Digital Signatures**: X.509 PKI certificate generation, SHA-256 integrity digest computation, cryptographic document sealing, and validation modal.
* **Redaction**: Blackout redaction overlay with permanent irreversible sanitization.
* **Password Protection**: 256-bit AES encryption permission flags.
* **Watermarks & Bates Numbering**: Diagonal opacity-controlled watermarks and sequential Bates legal numbering.

### 7. Print Production & CAD Tools
* Preflight compliance audit (PDF/A-1b, PDF/X-1a, PDF/E).
* Bleed & crop marks generation with trim boxes.
* 2-Up booklet imposition compiler.
* Calibrated CAD engineering measurement tools (distance ruler, perimeter, area polygon).

### 8. Progressive Web App (PWA)
* Standalone app manifest (`manifest.json`) and high-res vector icon (`icon.svg`).
* Full offline capability via Service Worker (`sw.js`).

---

## 🛠 Local Development

```bash
# Clone the repository
git clone <your-repo-url>
cd acrobat-reader-clone

# Start local server
python3 -m http.server 8080
# Open http://localhost:8080 in your browser
```

---

## 📄 License
This project is open-source under the [MIT License](LICENSE).
