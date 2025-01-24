# Gradual modality dropout using nnUnet

Incorporation of gradual modality dropout in nnUnet. Follow the installation (from source using this folder) and usage instructions from https://github.com/MIC-DKFZ/nnUNet 


## How to incorporate gradual modality dropout in the training phase?

Run nnUNetv2_train DATASET_NAME_OR_ID UNET_CONFIGURATION FOLD -*mod* -*prob* -*gradual*

### -mod

List of modalities where the method is going to be applied.

### -prob

Dropout probability

### -gradual

1 if it is gradual, 0 if it is applied fully (without smooth function)

Example: nnUNetv2_train 1 3d_fullres -mod 4,3 -prob 0.2 -gradual 1 
3d_fullres nnUnet training on dataset 1 applying gradual modality dropout in the modality 4 and 3 with probability 0.2
