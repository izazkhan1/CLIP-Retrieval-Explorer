@"
# CLIP Retrieval Explorer

A training-free cross-modal search system using OpenAI's CLIP model for multimodal retrieval.

## 🎯 Features

- **Text-to-Image Search**: Enter text, find matching images
- **Image-to-Image Search**: Find similar images by uploading reference
- **Image-to-Text Search**: Generate text descriptions for images
- **Fast Retrieval**: FAISS-based similarity search (sub-millisecond performance)
- **Visualization**: UMAP & t-SNE embedding space exploration
- **Clustering Analysis**: KMeans clustering of CLIP embeddings
- **Dark-Themed UI**: Custom Gradio interface with live metrics

## 📊 Performance Metrics

- **Recall@1**: 0.65
- **Recall@10**: 0.92
- **Dataset**: Flickr30k (~7,200 images)
- **Embedding Dimension**: 512 (CLIP ViT-B/32)

## 🛠️ Technologies

- Python 3.8+
- OpenAI CLIP
- FAISS (similarity search)
- UMAP & t-SNE (dimensionality reduction)
- KMeans (clustering)
- Gradio (UI)
- NumPy, Pandas

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Run Locally
```bash
python app.py
```

Then open: http://localhost:7860

## 📁 Project Structure

\`\`\`
clip-retrieval-explorer/
├── embeddings/          # Pre-computed CLIP embeddings
├── data/                # Flickr30k dataset
├── notebooks/           # Jupyter notebooks for exploration
├── app.py              # Main Gradio application
├── retrieval.py        # FAISS retrieval logic
├── visualization.py    # UMAP/t-SNE visualization
├── evaluation.py       # Metrics & benchmarking
└── requirements.txt
\`\`\`

## 📈 Evaluation Methodology

- Zero-shot retrieval evaluation on Flickr30k test set
- Metrics: Recall@K, Mean Reciprocal Rank (MRR)
- Failure analysis: 5 categories (negation, spatial reasoning, object counting, etc.)

## 🎓 Project Status

**Final Year Project** - University of Swat, Department of Computer Science  
**Team**: Izaz Ullah Khan (Roll: 2261130), Shahab Ahmad (Roll: 2261120), Jebran Khan (Roll: 2261104)  
**Supervisor**: Younas Ali  
**Expected Completion**: September/October 2026

## 📝 Failure Gallery

See \`docs/failure_cases.md\` for documented edge cases and limitations.

## 📧 Contact

- Email: I.zkhan0030@gmail.com
- GitHub: [Your GitHub Profile]

---

*Built with ❤️ for exploring the intersection of vision and language.*
"@ | Out-File README.md -Encoding UTF8
