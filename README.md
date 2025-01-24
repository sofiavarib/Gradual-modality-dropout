# Gradual modality dropout using nnUnet

Incorporation of gradual modality dropout in nnUnet. Follow the installation (from source using this folder) and usage instructions from https://github.com/MIC-DKFZ/nnUNet 


## How to incorporate gradual modality dropout in the training phase?

Run nnUNetv2_train DATASET_NAME_OR_ID UNET_CONFIGURATION FOLD -*mod* (modality to be applied, integer representing its position) -*prob* (probability for the dropout)
