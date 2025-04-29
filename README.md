# Brain Tumor Classification

This project focuses on classifying brain tumors using various deep learning models, including AlexNet, ResNet50, DenseNet169, Vision Transformer, and a custom CNN. The dataset used for training and evaluation contains MRI images of four classes: Glioma, Meningioma, Normal, and Pituitary.

## Project Structure

```
BRIAN_TUMOR_CLASSIFICATION/
│
├── dataset/
│   ├── Augmented/
│   │   ├── 512Glioma/
│   │   ├── 512Meningioma/
│   │   ├── 512Normal/
│   │   └── 512Pituitary/
│   ├── Raw/
│   │   ├── 512Glioma/
│   │   ├── 512Meningioma/
│   │   ├── 512Normal/
│   │   └── 512Pituitary/
│   └── dataset.csv
│
├── models/
│   ├── alexnet-model.ipynb
│   ├── custom_cnn.ipynb
│   ├── densenet169_model.ipynb
│   ├── resnet50_model.ipynb
│   └── vision_transformer_model.ipynb
│
├── .gitignore
├── EDA.ipynb
└── README.md
```

## Dataset

The dataset is structured into two main folders:
- `Raw/`: Contains the original MRI images.
- `Augmented/`: Contains augmented versions of the MRI images for better model generalization.

The dataset can be downloaded from Kaggle. Ensure you have the correct dataset uploaded to your Kaggle environment.

## Running the Project on Kaggle

To run the project locally, download the dataset from Kaggle and move the images into their corresponding directories according to the project directory. Another option is to run the code on Kaggle

### Step 1: Set Up the Kaggle Environment
1. Log in to your Kaggle account.
2. Create a new Kaggle notebook and import the notebook.
3. Importing the notebook may cause issues. If issues occur, create a new notebook, copy each cell, and run the notebook.
4. Enable GPU acceleration for faster training. Go to **Settings** > **Accelerator** and select the **P100 GPU**. 

### Step 2: Add the Dataset
1. Navigate to the **Add Data** section in your Kaggle notebook.
2. Search for the dataset "PMRAM Bangladeshi Brain Cancer - MRI Dataset" and add it to your notebook.

### Step 3: Run the Notebooks
1. Open the desired model notebook from the `models/` directory (e.g., `resnet50_model.ipynb`).
2. Update the dataset path in the notebook to match the Kaggle dataset directory if you're running the code on Kaggle:
   ```python
   dataset_root = "/kaggle/input/pmram-bangladeshi-brain-cancer-mri-dataset/PMRAM Bangladeshi Brain Cancer - MRI Dataset/PMRAM Bangladeshi Brain Cancer - MRI Dataset/Augmented Data/Augmented"  
    ```

## Authors

This project was created by a group of 3 AUS students:

- Saeed Bin Mizan
- Mohamed Monir Eltamamy
- Samad Sayed

## Disclaimer

- This final project was required for out Computer Vision Course at the American University of Sharjah.
- We utilized Generative AI tools such as ChatGPT for optimization of the codes and to enhance the efficiency of our development workflow. 