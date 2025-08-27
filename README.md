# 📚 Cold-Start Book Recommendation System (Hugging Face + FAISS + Gradio)

A **content-based book recommendation engine** that solves the **cold-start problem** — recommending books without user history.  
This project combines **Hugging Face transformer embeddings**, **FAISS vector search**, and **hybrid recommender logic** with an interactive **Gradio UI**.  

---

## ✨ Features
- **Dataset Preparation**  
  - Collected, merged, and balanced multiple book datasets across categories.  
  - Cleaned, normalized, and deduplicated text. 

Links For the Datasets 
Dataset 1 : https://www.kaggle.com/datasets/arpansri/books-summary
Dataset 2 : https://www.kaggle.com/datasets/ymaricar/cmu-book-summary-dataset

- **Transformer Embeddings**  
  - Used Hugging Face `sentence-transformers` (`all-mpnet-base-v2`) to encode **book titles + summaries** into dense semantic vectors.  

- **Vector Retrieval (FAISS)**  
  - Indexed embeddings using **FAISS** for efficient similarity search.  

- **Hybrid Recommendation Models**  
  - **Content-based similarity** (semantic nearest neighbors)  
  - **Category alignment** using Jaccard overlap  
  - **Diversity re-ranking** using Maximal Marginal Relevance (MMR)  

- **Interactive UI** (Gradio)  
  - Recommend by **category** (e.g., psychology, business, fiction)  
  - Find **“more like this”** (similar to a given book)  
  - **Hybrid mode** → mix of seed + category preferences  

---

## 🛠️ Tech Stack
- [Hugging Face Transformers](https://huggingface.co/transformers/)  
- [Sentence Transformers](https://www.sbert.net/)  
- [FAISS](https://github.com/facebookresearch/faiss)  
- [Gradio](https://www.gradio.app/)  
- Python (Pandas, NumPy, Scikit-learn)  

---
