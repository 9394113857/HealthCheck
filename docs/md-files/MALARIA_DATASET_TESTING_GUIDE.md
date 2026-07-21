# 🦟 Malaria Predictor - Sample Dataset Testing Guide

This guide explains exactly which files to download and which image files to upload for testing the Malaria Prediction model.

---

# Dataset 1 (Recommended)

## NIH Thin Blood Smear Dataset

Official Download Page

https://data.lhncbc.nlm.nih.gov/public/Malaria/NIH-NLM-ThinBloodSmearsPf/

---

## Download this file

```
NIH-NLM-ThinBloodSmearsPf.zip
```

Size

```
690 MB
```

---

## Do NOT download for prediction

These files are only documentation.

```
ReadMe.pdf

Dataset_statistics.xlsx

Data License Agreement.docx
```

---

## Extract ZIP

After extracting you'll get

```
NIH-NLM-ThinBloodSmearsPf/

│
├── Point Set/
├── Polygon Set/
├── ReadMe.pdf
├── Dataset_statistics.xlsx
└── Data License Agreement.docx
```

---

## Open

```
Point Set
```

Inside you'll see many folders like

```
292C144P105ThinF

345C162P123ThinF

378C239ThinF

520C145ThinF

612C98ThinF
```

Open any folder.

Example

```
Point Set/

└── 292C144P105ThinF/

        Img/
```

Now open

```
Img
```

You'll see microscope images like

```
000001.jpg

000002.jpg

000003.jpg

000004.jpg

000005.jpg
```

---

## Upload only these files

```
*.jpg
```

Example

```
000001.jpg

000015.jpg

000097.jpg
```

These are the files to upload into your website.

Expected Output

```
Parasitized

OR

Uninfected
```

depending on your trained model.

---

# Dataset 2 (Most Popular)

## Kaggle Cell Images Dataset

Download

https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria

Download

```
cell_images.zip
```

Extract.

You'll get

```
cell_images/

│

├── Parasitized/

└── Uninfected/
```

---

# Positive Test Images

Open

```
Parasitized
```

Example files

```
C33P1thinF_IMG_20150619_114756a_cell_179.png

C39P4thinF_original_IMG_20150622_105554_cell_31.png

C50P11thinF_IMG_20150724_114951_cell_148.png

C68P29N_ThinF_IMG_20150819_134112_cell_152.png

C99P60ThinF_IMG_20150918_141314_cell_117.png
```

Upload any of them.

Expected Prediction

```
Parasitized
```

---

# Negative Test Images

Open

```
Uninfected
```

Example files

```
C1_thinF_IMG_20150604_104722_cell_9.png

C2_thinF_IMG_20150604_114730_cell_15.png

C3_thinF_IMG_20150604_115700_cell_45.png

C5_thinF_IMG_20150609_122006_cell_31.png

C12NThinF_IMG_20150614_124212_cell_111.png
```

Upload any image.

Expected Prediction

```
Uninfected
```

---

# If Website Accepts JPG Only

Most Kaggle images are

```
PNG
```

Convert PNG → JPG using

https://convertio.co/png-jpg/

OR

https://www.iloveimg.com/convert-to-jpg

Then upload the JPG image.

---

# Which Dataset Should I Use?

If your model was trained using

```
cell_images/

    Parasitized/

    Uninfected/
```

then test using

```
Parasitized

Uninfected
```

images from Kaggle.

---

If your model was trained using

```
NIH-NLM-ThinBloodSmearsPf
```

then upload

```
Point Set/

Patient Folder/

Img/

*.jpg
```

files.

---

# Quick Testing Steps

1. Download dataset.

2. Extract ZIP.

3. Open image folder.

4. Select one blood cell image.

5. Open your Malaria Predictor website.

6. Click

```
Choose File
```

7. Upload image.

8. Click

```
Predict
```

9. Check prediction.

---

# Important

Do NOT upload

```
ZIP files

PDF files

Excel files

DOCX files
```

Only upload

```
.jpg

or

.png
```

blood cell microscope images.

---

# Need Help?

If prediction is wrong, share

```
app.py

model file (.keras/.h5/.pt/.pkl)

requirements.txt

prediction code

preprocessing code
```

and the complete project folder.

The preprocessing, image resizing, normalization, and class mapping can then be checked to ensure the uploaded images are handled correctly.
