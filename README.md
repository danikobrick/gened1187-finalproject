# gened1187-finalproject
Repository for Dani Kobrick's GENED1187 Final Project


All Jupyter notebooks were created in and meant to be run in Google Colab. You will need to accept the Google Drive mount to allow it to edit your drive. Running the code will create files to save the FER2013 dataset, the processed FER2013 dataset with only adults, filepaths for best checkpoints, and other forms of results. All files will appear in folders, and they will be saved to a folder called fer-project that will appear in the home of your Google Drive directory.

It is recommended to run these Jupyter notebooks on GPU, such as G4. Note -- the VGG model in particular can take an hour or more to train. 

Below is a description of each notebook and the sequence to run them in:

1. FER_data.ipynb: contains data retrieval, basic EDA, data processing
2. FER_CNN.ipynb: contains Baseline CNN model (with data augmentation) and gender bias analysis
3. FER_VGG_cyclical.ipynb: contains final VGG_cyclical model and gender bias analysis
4. FER_OTHER_models.ipynb: contains autoencoder model

Run the FER_data notebook first to download the data into your Drive, then you can run notebooks 2-4.

The folder fer-2013 contains all of the data from processing, the best checkpoints, and the stored paths. This is essentially what would be created when you run all the code. You can upload this folder to your Drive, and that way the code can use the cached paths. The models, however, would still take a long time to run.
