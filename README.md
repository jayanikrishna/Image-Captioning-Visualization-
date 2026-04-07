# Image-Captioning-Visualization-
An Affective Computing project using CLIP and BLIP to align AI-generated narratives with Baroque art.
# Baroque Art AI: Perception & Narrative Alignment
> **Status:** 🚧 Phase 1 (Perception Layer) Complete | Phase 2 (Narrative/Validation) In Progress

## 📌 Project Overview
This project explores the intersection of **Natural Language Processing (NLP)** and **Computer Vision** by generating stories that are mathematically aligned with historical Baroque artwork.

## 🛠️ Phase 1: Perception Layer (My Role)
As **Member 1**, I built the extraction pipeline to provide the project's visual "Ground Truth."

### **Technical Implementation:**
* **Dataset:** WikiArt Baroque collection (~4,240 images).
* **Feature Extraction:** Used **OpenAI's CLIP (ViT-B/32)** to generate 512-dimensional embeddings.
* **Normalization:** Applied **L2-Normalization** to ensure vectors are ready for Cosine Similarity validation.
* **Captioning:** Utilized **Salesforce's BLIP** for factual image descriptions to prevent narrative hallucinations.
* **Efficiency:** Designed a chunked processing loop that saves progress every 500 images to manage T4 GPU memory.

## 📂 Deliverables
- [x] **member1_baroque_parts_1-9.json:** 512-d unit vectors and factual captions for the entire dataset.
- [ ] **Phase 2:** Narrative Generation (Member 2).
- [ ] **Phase 3:** Cosine Similarity Validation (Member 4).

## 🧰 Tech Stack
- PyTorch, Transformers (HuggingFace), NumPy, PIL, KaggleHub.
