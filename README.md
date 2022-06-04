# Explainable Wound Classification
This project trains and evaluates different [CMSF](https://github.com/UMBCvision/CMSF) models for the task of classifying images from a mouse wound dataset into one of the four biological stages of healing. Explanability was achieved by generating saliency maps with [RISE](https://github.com/eclique/RISE) and analyzing how transforming the input images affect the models' predictions. All notebooks were written to be run in Google Colab.

## Repository Contents

### Data Folders
[Cropped images](Cropped images) The original dataset of mouse wound images.
[Circle_Cropped_images](Circle_Cropped_images) Circular crops of the mouse wound images.
[Split_images](Split_images) The circular images split into training, validation, and test data

### Notebooks
[Image Processing.ipynb](Image Processing.ipynb) Generates the circularly cropped images
[Split images.ipynb](Split images.ipynb) Splits the circularly copped images into train, validtion, and test data
[HealNet Pretrain.ipynb](HealNet Pretrain.ipynb) Pretrains the Resnet18 encoders used in the CMSF models
[CMSF tests.ipynb](CMSF tests.ipynb) Performs label cleaning and all the main CMSF trainings and experiments

### Misc Files
[Updated_Cropped_Images_Wound_Stage_Probabilities.csv](Updated_Cropped_Images_Wound_Stage_Probabilities.csv) Soft wound stagelabels for the data
[Cleaned_Wound_Stage_Labels.csv](Cleaned_Wound_Stage_Labels.csv) The soft wound labels with the cleaned hard labels generated by [CMSF tests.ipynb](CMSF tests.ipynb)
[resnet_healnet_encoder_weights.tar](resnet_healnet_encoder_weights.tar) The pretrained encoder weights generated by [HealNet Pretrain.ipynb](HealNet Pretrain.ipynb)

### Copied Files
[CMSF](CMSF) Select files copied from the [CMSF](https://github.com/UMBCvision/CMSF) repository
[RISE](RISE) A copy of the [RISE](https://github.com/eclique/RISE) repository