{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "3f82ecfc-b8e5-4903-bd4a-ed778f3b686e",
   "metadata": {},
   "source": [
    "# Multimodal Search Engine with SOM Visualization\n",
    "\n",
    "This project implements a cross-modal search engine connecting images, video frames, and textual content. It integrates Self-Organizing Maps (SOMs) for visualization and semantic clustering across domains.\n",
    "\n",
    "---\n",
    "\n",
    "## 📁 Project Structure\n",
    "\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "462cdaf0-5b13-4fb3-8fc4-6e9d28408b4b",
   "metadata": {},
   "source": [
    "├── main.ipynb # Main notebook entry point\n",
    "├── vectorisation_comparison.py # TF-IDF vs SBERT comparison\n",
    "├── train_clip_som_with_qe_te.py\n",
    "├── train_sbert_som_with_qe_te.py\n",
    "├── plot_som_rgb_comparison.py\n",
    "├── plot_sbert_som_rgb_comparison.py\n",
    "├── generate_mixed_search_groups.py\n",
    "├── image/processed/ # CLIP image features\n",
    "├── text/ # SBERT PDF text features\n",
    "├── subset/ # Processed subset of frames/captions\n",
    "└── SOM/ # SOM outputs (lattices, plots, summaries)"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "9c0a863f-f720-4a62-b0ab-a9d8ca531523",
   "metadata": {},
   "source": [
    "\n",
    "---\n",
    "\n",
    "## Setup Instructions\n",
    "\n",
    "1. Clone the repo and install dependencies:\n",
    "\n",
    "```bash\n",
    "git clone https://github.com/yourname/your-repo.git\n",
    "cd your-repo\n",
    "pip install -r requirements.txt\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "93f7acd1-41d3-4cb5-a72a-13ef008b2d96",
   "metadata": {},
   "source": [
    "\n",
    "---\n",
    "\n",
    "## How to Run\n",
    "In main.ipynb:\n",
    "\n",
    "View vectorisation results\n",
    "\n",
    "Run CLIP + SBERT SOM training with QE/TE\n",
    "\n",
    "Visualize RGB SOMs\n",
    "\n",
    "Perform and visualize search paths\n",
    "\n",
    "Review final conclusions"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "29f63a90-3e5b-4296-a97b-dcf81dc2c30f",
   "metadata": {},
   "source": [
    "\n",
    "---\n",
    "\n",
    "## Output Samples\n",
    "qe_te_clip.png, qe_te_sbert.png — Training error curves\n",
    "\n",
    "clip_som_rgb_comparison.png, sbert_som_rgb_comparison.png — PCA RGB SOM maps\n",
    "\n",
    "mixed_clip_som.png, mixed_sbert_som.png — Activation maps\n",
    "\n",
    "mixed_search_summary.csv — Full search result paths"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "8ad65a33-08e0-46a7-9af2-dc977f3f63b2",
   "metadata": {},
   "source": [
    "---\n",
    "\n",
    "## Completed Requirements\n",
    " 3 datasets, 2+ domains\n",
    "\n",
    " Custom search engine from multiple sources\n",
    "\n",
    " SOMs per domain with 10+ activation examples\n",
    "\n",
    " QE / TE tracking and best lattice selection\n",
    "\n",
    " PCA RGB SOM visualization (2 methods)\n",
    "\n",
    " Vectorisation comparison (TF-IDF vs SBERT)\n",
    "\n",
    " Notebook structured and reproducible\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "54eaa1a7-a526-45d4-a3f1-0b5bd7555e48",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python (sam-env)",
   "language": "python",
   "name": "sam-env"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.10.16"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
