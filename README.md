# Cosmoscope SOI 2023

## Description
This is a machine learning project used to analyse GCMS data collected by Sample Analysis at Mars (SAM) instrument. The goal is to detect the presence of various chemical compounds in samples.  

## Usage 
1. install required libraries
   ```bash
    $ pip install -r requirements.txt
   ```
2. edit the path varibles according to working enviornment in the cnn_model.ipynb and predictor.ipynb files.
    ``` bash
    # for working in kaggle use this paths
    # kag_path_in = "/kaggle/input/<data-set-name-in-kaggle>/"
    # kag_path_out = "/kaggle/working/"
    
    # # for working in colab  
    # kag_path_in = "/content/drive/MyDrive/" # google drive
    # kag_path_out = ""
    
    # for working locally (uncomment)
    kag_path_in = ""
    kag_path_out = ""
    ```
    use above code in the 4th code cell of cnn_model.ipynb and predictor.ipynb files if working locally 
4. run the cnn_model.ipynb file to generate the model file (cnn_model.keras) or download the model file from this [link](https://drive.google.com/file/d/1wTPzWdMYUIHmpdxTXdA7XWmaheo8O1gr/view?usp=sharing)
5. run the predictor.ipynb file to generate the prediction file (predictions.csv) or use the existing predictions.csv file for testing  

## Files

|main files                   | description|
|-----                   | ----|
|cnn_model.ipynb                   | main model|
|predictor.ipynb                   | for making predictions|
|requirements.txt                  |   |
|val_labels_Shlorp.csv                   | final prediction file|\

   |optional files                   | description|
   |-----                   | ----|
   |data_limit.ipynb                  | getting extreme values
   |logistic_regression_model.ipynb   | old logistic regression model
   |combined_cnn.ipynb                | old cnn model
   |peaks_and_common_values.ipynb     | for visualization and peak detection
   |plottingPeaks.ipynb               | visualization|
   |cnn_model_testing.ipynb           | used for finding best model achitecture|
