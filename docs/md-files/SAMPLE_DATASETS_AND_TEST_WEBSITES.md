# 🦟 Malaria Predictor - Sample Datasets & Public Testing Websites

This guide provides direct dataset download links, sample image folders, and public demo websites for testing your Malaria Prediction model.

---

# 📂 1. NIH Thin Blood Smear Dataset (Official)

## 🌐 Official Dataset Page

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/

## 📥 Download Complete Dataset

**File Name**

```
NIH-NLM-ThinBloodSmearsPf.zip
```

**Size**

```
690 MB
```

**Direct Download**

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/NIH-NLM-ThinBloodSmearsPf.zip

---

## ❌ Files NOT Used for Prediction

These files are documentation only.

```
ReadMe.pdf

Dataset_statistics.xlsx

Data License Agreement.docx
```

Never upload these files.

---

# 📸 2. Direct Sample Image Folders

You can download individual JPG images without downloading the full dataset.

---

## Folder 1

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/Point%20Set/292C144P105ThinF/Img/

Example Images

```
IMG_20151015_155004.jpg

IMG_20151015_155149.jpg

IMG_20151015_160529.jpg

IMG_20151015_160908.jpg

IMG_20151015_163142.jpg
```

---

## Folder 2

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/Point%20Set/345C162P123ThinF/Img/

Example Images

```
IMG_20151116_102655.jpg

IMG_20151116_102751.jpg

IMG_20151116_104114.jpg

IMG_20151116_104342.jpg

IMG_20151116_104451.jpg
```

---

## Folder 3

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/Point%20Set/378C239ThinF/Img/

Example Images

```
IMG_20151127_113008.jpg

IMG_20151127_113150.jpg

IMG_20151127_113202.jpg

IMG_20151127_113223.jpg

IMG_20151127_113253.jpg
```

---

## Folder 4

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/Point%20Set/204C63P24N_ThinF/Img/

Example Images

```
IMG_20150818_142948.jpg

IMG_20150818_143319.jpg

IMG_20150818_143423.jpg

IMG_20150818_143544.jpg

IMG_20150818_143757.jpg
```

---

# 📦 3. Kaggle Cell Images Dataset

## Dataset

https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria

Download

```
cell_images.zip
```

After extracting

```
cell_images/

├── Parasitized/
└── Uninfected/
```

---

## ✅ Positive Samples

```
C33P1thinF_IMG_20150619_114756a_cell_179.png

C39P4thinF_original_IMG_20150622_105554_cell_31.png

C50P11thinF_IMG_20150724_114951_cell_148.png

C68P29N_ThinF_IMG_20150819_134112_cell_152.png
```

Expected Prediction

```
Parasitized
```

---

## ✅ Negative Samples

```
C1_thinF_IMG_20150604_104722_cell_9.png

C2_thinF_IMG_20150604_114730_cell_15.png

C3_thinF_IMG_20150604_115700_cell_45.png

C5_thinF_IMG_20150609_122006_cell_31.png
```

Expected Prediction

```
Uninfected
```

---

# 🌐 4. Public Malaria Detection Demo Websites

## Hugging Face Spaces

https://huggingface.co/spaces?search=malaria

## Malaria Classifier Search

https://huggingface.co/spaces?search=malaria+classifier

> These pages list community malaria detection demos. Availability may change over time.

---

# 📤 Upload Rules

Upload ONLY

```
.jpg

.png
```

Do NOT upload

```
.zip

.pdf

.xlsx

.docx
```

---

# 🚀 Quick Testing Steps

1. Download a sample image.
2. Open your Malaria Predictor website.
3. Click **Choose File**.
4. Select a blood cell image.
5. Click **Predict**.
6. Verify the prediction.

---

# ✅ Recommended Testing Order

1. NIH Dataset ZIP
2. NIH Sample JPG Images
3. Kaggle Cell Images
4. Compare predictions using public demo websites

---

# 📄 Recommended Markdown File Name

```
SAMPLE_DATASETS_AND_TEST_WEBSITES.md
```
