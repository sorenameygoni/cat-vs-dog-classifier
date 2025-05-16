# 🐱 Cat vs Dog Classifier with ResNet18

This repository contains a deep learning project that classifies images of cats and dogs using a fine-tuned ResNet18 model in PyTorch. The model is trained on 25,000 images with various modern techniques to improve performance and robustness.

---

## 📌 Project Summary

- **Dataset Size:** 25,000 images (cats and dogs)
- **Architecture:** ResNet18 (pretrained on ImageNet)
- **Loss Function:** Custom Focal Loss with Label Smoothing
- **Optimizer:** AdamW
- **Scheduler:** Cosine Annealing
- **Augmentations:** Implemented using Kornia
- **Mixed Precision:** Enabled via AMP (Automatic Mixed Precision)
- **Best Validation Accuracy:** ~97%

---

## 📁 Folder Structure

```
tamrinecatdog/
├── PetImages/            # Training images
├── ValidationImages/     # Validation images
├── Test/                 # Test images
├── notebook.ipynb        # Jupyter Notebook with full pipeline
├── best_model.pth        # Saved best model
├── README.md             # Project documentation
├── requirements.txt      # Dependencies
```

---

## 🔧 Features & Techniques Used

| Technique               | Used |
|------------------------|------|
| Data Augmentation      | ✅   |
| Kornia for Augmentation| ✅   |
| ResNet18 (Pretrained)  | ✅   |
| Focal Loss             | ✅   |
| Label Smoothing        | ✅   |
| Cosine Annealing LR    | ✅   |
| AMP (autocast + scaler)| ✅   |
| ResNet Layer Freezing  | ✅   |

---

## 📈 Accuracy Plot

Validation and training accuracy were tracked over 35 epochs. LR and label smoothing were changed at epoch 25.

![Accuracy Plot](accuracy_plot.png)

---

## 🚀 Future Work

- Explore more powerful models such as **ResNet50** or **EfficientNet**.
- Implement a more advanced experiment tracking system (e.g., Weights & Biases or TensorBoard).
- Use Grad-CAM for visualizing model attention.

---

## 🛠 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/cat-vs-dog-classifier.git
cd cat-vs-dog-classifier
pip install -r requirements.txt
```

Make sure you have the dataset located in the appropriate folders.

---

## 🖥 Requirements

See the `requirements.txt` file.

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---
### 📥 Download Trained Model

You can download the best trained model (`best_model.pth`) from [Google Drive](https://drive.google.com/file/d/1zlu0zzOX6606yiiZzTuq1H-Mjd6habQ_/view?usp=drive_link).
Place it in the project root directory so it can be loaded easily for inference or testing.
______________________________________________________________________________________________

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
