# LexVerify AI: Legal Document Validator (v3.0)

**LexVerify AI** is an intelligent, browser-based legal document auditor. It uses **:contentReference[oaicite:0]{index=0} Gemini AI** to perform deep *legal reasoning* on contracts—identifying missing mandatory clauses, onerous payment terms, aggressive clawback provisions, and prohibited restrictive covenants.

---

## 🚀 Key Features

- **AI-Powered Validation**  
  Analyzes text for legal risks using the **Gemini 2.5 Flash** model.

- **OCR Support**  
  Built-in **Tesseract.js** integration allows users to upload images (JPG/PNG) of physical documents for text extraction.

- **PDF Intelligence**  
  Integrated **pdf.js** for direct text extraction from multi-page PDF documents.

- **Risk Categorization**  
  Specifically flags:
  - **Onerous Clauses**: Unfairly burdensome payment or liability terms  
  - **Clawback Provisions**: Aggressive recovery of bonuses or fees  
  - **Prohibited Terms**: Illegal non-competes or restraint of trade

- **Privacy-First**  
  API keys are stored in your browser’s `localStorage` and never sent to a backend server. OCR and PDF processing happen entirely on the client side.

---

## 🛠️ Tech Stack

- **Frontend**: React.js with Tailwind CSS  
- **Icons**: Lucide React  
- **AI**: Google Gemini API  
- **OCR**: Tesseract.js  
- **PDF**: PDF.js (`pdfjs-dist`)

---

## 📦 Installation & Local Setup

To run this project locally, follow these steps:

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/lexverify-ai.git
   cd lexverify-ai
