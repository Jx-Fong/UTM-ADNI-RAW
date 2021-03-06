# UTM-ADNI-RAW

1. UTM-ADNI-RAW is a collection of raw sagittal MRI slices obtained from ADNI dataset using simple search function. At the time being, UTM-ADNI-RAW only collect two classes which is Alzheimer Disease (AD) and Normal Control (NC). Both AD and NC have 500 dicom series per class, and for every series there are 166-180 dicom slices. 

2. Note: For MPR_AD_500, if you extract and seperate all files which contained dicom slices, you will only get 499 files, however one of the file will contain 2 dicom series (Eg. AD-441), summing up to a total of 500 dicom series. (ADNI database naming issue)

3. In order to save disk space while preserving the ability to preview image slices, we provide MRI images in DICOM-16bit and PNG-16bit format.

4. Both AD and NC data are combined into one folder and then further converted into MXNET RecordIO format (.rec) to speed up training. If you are using other frameworks (eg. TF), we do provide the original train/test image in PNG-16bit format.

5. From our internal testing, using 8-bit images instead of 16-bit images for training has no penalty in performance. Any further investigation or research on MRI bit-depth vs accuracy is welcomed.

#################################################################################################

Dataset URL: 
- 192.168.0.113/gitlab-cairo/utm-adni-raw (internal ip)
- gitlab.com/inokaicairo/UTM-ADNI-AD (temp)
- gitlab.com/inokaicairo/UTM-ADNI-NC (temp)

Update 1/1/2020: Currently UTM CAIRO server is in maintainance. A new url link to the dataset will be given after our staff setup a new domain address for the dataset.

Update 8/1/2020: Temporary link of final filtered and labeled dataset is updated. Full dataset (40GB) including original 500 AD and NC data will be provided with a new link in the future.
