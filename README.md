# Eye Disease Detection Project

This repository contains the code and files for the **Eye Disease Detection** project. The project aims to predict various eye diseases from retinal fundus images using machine learning models.

## Dataset

The dataset used for this project is the **Retinal Fundus Image Dataset** containing 50,000 images, categorized into 7 classes (6 diseases and 1 normal fundus). You can access and download the dataset from Kaggle:

[Retinal Fundus Image Dataset (50k images)](https://www.kaggle.com/datasets/gautamrajiitk/retinal-fundus-image-50k)

## Folder Structure

The final zip file contains 3 folders:

### 1. **Demo App**
This folder contains the code for the eye disease detection app. The app is built using **Streamlit**, which allows you to upload a retinal fundus image and receive a prediction of the most probable eye disease.

### 2. **Experiments Models**
This folder contains code for various experiments and models we tried during the development of the project. Some of these experiments were not saved, or were overwritten, but the available code can be useful for reference.

### 3. **Final Code**
This folder contains subfolders for different eye diseases, each containing:
- A Python notebook for training and testing the model for that specific disease.
- The resultant trained models.

#### Subfolders in **Final Code**:

- **AMD**: Contains the code for predicting Age-Related Macular Degeneration (AMD).
- **Cataract**: Contains the code for predicting Cataract.
- **DR**: Contains the code for Diabetic Retinopathy (DR).
- **Glaucoma**: Contains the code for Glaucoma.
- **Knowledge_Distillation**: Contains the code for implementing Knowledge Distillation (KD).
- **Pathological_Myopia**: Contains the code for predicting Pathological Myopia.
- **Vision_Transformer Combine**: Contains the code for predicting multiple diseases at once using Vision Transformer.

## How to Run the Various Files

### Running the Notebooks (Google Colab)
You can run the notebooks to train/test the models or directly load the saved models for inference.

1. Open the notebook (`.ipynb`) inside the respective disease folder.
2. Set the runtime to GPU:
   - `Runtime` → `Change runtime type` → Select **GPU**.
3. Open the notebook in Google Colab or upload it directly.
4. The dataset will be auto-downloaded using **gdown**.

   If for any reason, the download doesn't work, you can manually download the dataset from Kaggle using the following link:
   - [Download the Retinal Fundus Image Dataset (50k images)](https://www.kaggle.com/datasets/gautamrajiitk/retinal-fundus-image-50k)

5. Run all cells:
   - `Runtime` → `Run all`.
6. The model will train and the `.keras` file will be saved in the respective folder.

### Running the Streamlit Demo App
1. Go to the **Demo App** folder.
2. Open the terminal and run:
   ```bash
   streamlit run Final_Disease.py
