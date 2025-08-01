
# Facial Features Detection Project

This project detects facial attributes using deep learning:
- 👤 Gender (Male/Female)
- 🕶️ Wearing Glasses (Yes/No)
- 👕 Shirt Color (Red, Green, Blue, White, Black)

---

## 📁 Files Included

- `Problem1_Detecting Facial Features.ipynb` – The complete Google Colab notebook
- `gender_glasses_model.h5` – Trained model weights
- `Facial_Features_Detection_Presentation.pptx` – Presentation file
- `README.txt` – This file (instructions)
- Folder `/celeba/` containing:
  - `img_align_celeba/` – Aligned images (unzipped)
  - `list_attr_celeba.txt` – Attribute labels

---

## 🚀 How to Run

1. **Upload files to Google Drive**  
   - Create a folder `celeba` in your `My Drive`  
   - Upload `img_align_celeba.zip` and `list_attr_celeba.txt`  
   - Unzip the images inside `/celeba/` so the path becomes:
     ```
     /content/drive/MyDrive/celeba/img_align_celeba/
     ```

2. **Open the notebook in Google Colab**
   - Mount Google Drive:  
     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```

3. **Run the notebook cells one by one**
   - Make sure the model is trained or load `gender_glasses_model.h5` to skip training.

4. **Upload Your Image**
   - Use the last cell to upload any image.
   - Output: Gender, Glasses, Shirt Color and Displayed Image

---

## 📦 Output Example

```
👤 Gender: Female  
🕶️ Glasses: Yes  
👕 Shirt Color: Blue  
```

---

## ⚠️ Notes

- Use aligned and front-facing images for best accuracy.
- Shirt detection depends on visibility in lower half of image.
- Model is trained on 10k samples, for demo/testing purpose only.


