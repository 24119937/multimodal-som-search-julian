# Multimodal Search Engine with SOM Visualization

This project implements a cross-modal search engine connecting images, video frames, and textual content. It integrates Self-Organizing Maps (SOMs) for visualization and semantic clustering across domains.

---

## Project Structure

```
├── main.ipynb                     # Main notebook entry point
├── requirements.txt              # Python dependencies
├── vectorisation_comparison.py   # TF-IDF vs SBERT comparison
├── train_clip_som_with_qe_te.py
├── train_sbert_som_with_qe_te.py
├── plot_som_rgb_comparison.py
├── plot_sbert_som_rgb_comparison.py
├── generate_mixed_search_groups.py
├── image/processed/              # CLIP image features
├── text/                         # SBERT PDF text features
├── subset/                       # Subset of frames and captions
└── SOM/                          # SOM outputs (lattices, plots, summaries)
```

---

## Setup Instructions

```bash
git clone https://github.com/24119937/multimodal-som-search-julian.git
cd multimodal-som-search-julian
pip install -r requirements.txt
```

---

## How to Run

Open `main.ipynb` and follow these steps:

1. View vectorisation comparison (SBERT vs TF-IDF)
2. Run CLIP and SBERT SOM training with QE/TE tracking
3. Visualize SOMs with RGB PCA (two methods)
4. Perform multimodal search (image, frame, text)
5. Review search results and final conclusions

---

## Output Samples

- `qe_te_clip.png`, `qe_te_sbert.png` — Training error curves
- `clip_som_rgb_comparison.png`, `sbert_som_rgb_comparison.png` — PCA RGB SOM visualizations
- `mixed_clip_som.png`, `mixed_sbert_som.png` — SOM activation maps
- `mixed_search_summary.csv` — Full search result paths across modalities

---

## Completed Requirements

- 3 datasets from at least 2 domains (image and text)
- Custom search engine with multiple input types
- One SOM per domain with activation tracking
- QE and TE analysis with best SOM selection
- RGB SOM visualization using two PCA methods
- Vectorisation method comparison (SBERT vs TF-IDF)
- Structured and reproducible notebook implementation
