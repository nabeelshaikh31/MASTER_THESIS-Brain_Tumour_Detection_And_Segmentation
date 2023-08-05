# MASTER_THESIS-Brain_Tumour_Detection_And_Segmentation

Brain tumour diagnosis, prognosis, and treatment all greatly benefit from accurate segmentation of several sub-areas of gliomas such as necrotic and non-enhancing tumour core, peritumoral edema, and enhancing tumour core from multi-channel MRI images. However, semantic segmentation of these sub-regions has always been a challenging part due to the brain’s anatomical structure.
In these circumstances, several semantic and medical image segmentation tasks have become simpler thanks to deep learning algorithms, a large number of which are based on the UNET architecture with symmetric contraction and expansion path for end-to-end segmentation. With the aid of these computer vision techniques, we have improved the success rate of tumour segmentation due to its great effectiveness and solid performance.
In this paper, we propose segmenting necrotic and non-enhancing tumour core, peritumoral edema, and enhancing tumour core, which are the sub-areas of Gliomas, by combining various techniques such as 3D MRI, 3D UNET, and Residual UNET architecture method.

## BraTS2020 Dataset:

The evaluation of cutting-edge techniques for the segmentation of brain tumours in multimodal magnetic resonance imaging (MRI) scans has always been the main emphasis of BraTS. The most recent version (2020) of the BRATS training dataset contains 369 multi-modality MRI scans, of which 293 were obtained from patients with glioblastoma (GBM/HGG) and 76 from lower grade glioma (LGG), together with their ground truth segmentations for evaluation. 
All BraTS multimodal scans are accessible as NIfTI files (.nii.gz). Fluid Attenuated Inversion Recovery (FLAIR), T2-weighted MRI (T2), T1-weighted MRI (T1), T1-weighted MRI with gadolinium contrast enhancement (T1ce) are the four common MRI channels used to detect and segment gliomas and were obtained using multiple clinical protocols and scanners from various institutions. Annotations in BraTS dataset include the necrotic and non–enhancing tumour core (NCR/NET — label 1), the peritumoral edema (ED — label 2), and the GD– enhancing tumour (ET — label 4).
We can download the BraTS2020 dataset from Kaggle.

#### NOTE: Let us make a minor correction in the dataset before moving forward to the next step. Inside the dataset folder, go to "./MICCAI_BraTS2020_TrainingData/". Inside that folder go to "BraTS20_Training_355" and inside of that You will find 5 .nii files. There should be 4 files ending with t1, t1ce, t2, flair. However, the last remaining file will have a random name which does not match with any other image folder. Therefore, please rename it to "BraTS20_Training_355_seg.nii". We do this so that every image is consistent throughout and all have 5 files ending with t1, t1ce, t2, flair and seg.


# NOTE: The entire code is very well structured and self explanatory with relevant comments and explanations provided after each line of code for better and clear understanding of the whole concept.
