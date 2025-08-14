# 🫁 RSNA Pneumonia Detection Challenge

This repository contains a deep learning project based on the [RSNA Pneumonia Detection Challenge](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge), which aims to detect pneumonia in chest X-rays using object detection techniques.

---

## 📦 Dataset

The dataset used is provided by the Radiological Society of North America (RSNA) via Kaggle.

🔗 [RSNA Pneumonia Detection Challenge on Kaggle](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge)

### ❗ Data Not Included

Due to privacy concerns, the dataset is **not included** in this repository. To use it:

1. Sign in to [Kaggle](https://www.kaggle.com/)
2. Accept the competition rules
3. Download the dataset manually
4. Place it in the `data/` directory as follows:

```
data/
├── stage_2_train_images/             # DICOM images
├── stage_2_train_labels.csv
├── stage_2_detailed_class_info.csv
└── sample_submission.csv
```

---

## 📁 Project Structure

```
rsna-pneumonia-detection/
│
├── notebooks/
│   └── preprocessing.ipynb              # Jupyter notebook for preprocessing stage
│   └── pneumonia_detection.ipynb        # Jupyter notebook for training and evaluation
│   └── interpretability.ipynb           # Jupyter notebook for interpretability of model
│
├── data/
│   └── README.md                        # Instructions for setting up the dataset
│
├── requirements.txt                     # Python dependencies
├── environment.yml                      # Conda environment (optional)
├── .gitignore
├── LICENSE
└── README.md
```

---

## ⚙️ Installation

### Using pip

```bash
pip install -r requirements.txt
```

### Using conda (optional)

```bash
conda env create -f pytorch_env_windows.yml
conda activate pytorchenv
```

---

## 🚀 Usage

### Run the notebook:

```bash
jupyter notebook notebooks/pneumonia_detection.ipynb
```

### Convert and run as Python script:

```bash
jupyter nbconvert --to script notebooks/pneumonia_detection.ipynb
python notebooks/pneumonia_detection.py
```

---

## 🧠 Model

The model used is a convolutional neural network (CNN) designed for object detection.

### Features:
- Preprocessing of DICOM images
- Visualizations for interpretability

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

This project is intended **for educational and research purposes only**. It is **not suitable for clinical decision-making** or medical use.

---

## 🙏 Acknowledgements

- [RSNA](https://www.rsna.org/) and [SIIM](https://siim.org/) for advancing research and education in medical imaging  
- [Kaggle](https://www.kaggle.com/) for hosting the RSNA medical imaging challenges  
- Udemy course **“Deep Learning with PyTorch for Medical Image Analysis”** by **Jose Portilla**, **Marcel Früh**, **Sergios Gatidis**, and **Tobias Hepp**, for hands‑on training in applying deep learning to medical imaging, including DICOM/NIfTI data handling, tumor segmentation, and interpretability 
- Public contributors, open‑source developers, and the research community driving innovation in radiology AI  
- All patients and institutions that contributed anonymized data for public use  
