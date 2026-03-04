# LLM-Driven Building Life Cycle Assessment (LCA)

### Research Context
This project leverages Large Language Models (LLMs) to automate and refine the estimation of embodied carbon in the built environment. By integrating unstructured research data (PDFs), practice guides (Text), and building datasets (Excel), this tool uses **In-Context Learning** to provide plausible LCA ranges for diverse building types.

---

## 🚀 Key Features
* **Multi-Modal Data Ingestion:** Automates text extraction from PDFs, Excel glossaries, and practice guidelines.
* **Stanford API Integration:** Orchestrates calls to `Claude-3-7-Sonnet` via the Stanford API Gateway.
* **Batch Processing:** Logic to handle large building datasets in chunks to optimize API rate limits and stability.
* **Structured Output:** Automatically extracts LLM-generated markdown tables and saves them into versioned Excel sheets.

---

## 📁 Project Structure


```text
building-lca-llm/
├── data/
│   ├── articles/          # Research papers (PDFs)
│   ├── Excel/             # Input building data and glossaries
│   └── results/           # Generated LCA estimates
├── src/
│   └── lca_incontext.ipynb # Exploratory research notebook
├── .env.example           # Template for API credentials
├── .gitignore             # Ensures private data and keys stay local
└── requirements.txt       # Project dependencies