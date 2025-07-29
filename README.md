# 🖼️ Image Retrieval Project (Experiment)

An experimental image retrieval system for evaluating how different deep learning models represent image features for visual similarity search.

## 🚀 Objectives
- Compare feature extraction quality between CNN-based (e.g., VGG19, Resnet50) and Transformer-based (e.g., ViT) models
- Build a simple, interactive system to test real-time image retrieval performance
- Identify which model backbone is more suitable for feature-based image retrieval tasks

## 📊 Evaluation Criteria
- 🎯 **Top-k Accuracy**: How often the correct or most similar image(s) appear in the top-k results

## 🧪 Experimental Setup
- Feature extractors: `VGG19`,`Resnet50`, `ViT (vit_base_patch16_224)`
- Dataset: Custom image set in `/Data/`
- Retrieval metric: `Cosine similarity`

## 🧰 Tech Stack
- Python
- Pytorch
- NumPy, OpenCV

## 🗂️ Project Structure
```
Image_Retrieval_Project/
│
├── Data/ # Image dataset
├── Model/ # Saved models or model-related files
└── requirements.txt # Required Python packages
```
## 📈 Preliminary Results

| Model     | Feature Dim | Top-5 Accuracy | Notes               |
|-----------|-------------|----------------|---------------------|
| VGG19     | 512         | 74%            | CNN baseline        |
| Resnet50  | 2048        | 82%            | Deeper CNN, better performance|
| ViT-B/16  | 768         | 89%            | Better generalization |
