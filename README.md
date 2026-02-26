# LexVerify AI: Legal Document Validator (v3.1)

**LexVerify AI** is a high-performance, browser-based legal document auditor. It leverages **:contentReference[oaicite:0]{index=0} Gemini 2.5 Flash AI** to perform deep *legal reasoning* on contracts—identifying missing mandatory clauses, onerous payment terms, aggressive clawback provisions, and prohibited restrictive covenants.

---

## 🚀 Key Features

- **AI-Powered Validation**  
  Deep analysis of contract text using the **Gemini 2.5 Flash** model with structured JSON output.

- **Built-in OCR Support**  
  Integrated **Tesseract.js** allows users to upload images (JPG/PNG) of physical documents for instant text extraction.

- **Native PDF Reading**  
  Integrated **PDF.js** for direct text extraction from multi-page PDF documents without server-side processing.

- **Risk Categorization**  
  Specifically trained to flag:
  - **Onerous Clauses**: Unfairly burdensome payment or liability terms  
  - **Clawback Provisions**: Aggressive recovery of bonuses or fees  
  - **Prohibited Terms**: Illegal non-competes or restraint of trade

- **Robust Error Handling**  
  Implements exponential backoff and retry logic for API calls to ensure stability under heavy load or poor network conditions.

- **Privacy-First**  
  API keys are stored in your browser’s `localStorage`. OCR and PDF processing happen entirely on the client side.

---

## 🛠️ Tech Stack

- **UI Framework**: Tailwind CSS (via CDN)  
- **Icons**: Lucide Icons  
- **AI Engine**: Google Gemini API (v1beta)  
- **OCR Engine**: Tesseract.js  
- **PDF Engine**: PDF.js (`pdfjs-dist`)

---

## 📦 Deployment Options

### Option 1: Standalone (Recommended for GitHub Pages)

This project is designed to run as a single, self-contained `index.html` file.

1. Create a new repository on GitHub.  
2. Upload your `index.html` file.  
3. Go to **Settings → Pages** and enable hosting from the main branch.  
4. 🎉 Your app is live!

### Option 2: Local Setup (Developer Mode)

1. Clone the repository.  
2. Open `index.html` directly in any modern web browser.  

**Alternatively, use a local server:**
```bash
# If you have Python installed
python -m http.server 8000
