# matlab_journey
This is a simple introduction to matlab for image analysis. The codes used here require installation of image processing toolbox, deep learning toolbox. 

Volume: This part deals with calculation of volume of a binary mask containing ones and zeroes. The file Niti_vol.m also contains codes in R and fsl for performing the same task are also provided.

```matlab
matlab
ImN='test.nii'; %assign ImN 
Roi=niftiread(ImN); %Roi is handle for image
Roi=Roi>0.5; %ensure binary mask
rp=regionprops3(Roi) %find properties of volume data
```

TSNE: This part deals with calculation of centre of gravity of a binary image. The file tsne_image.m illustrates the use of random number to create 3D array and 3D plot with scatter3. T-stochastic neighbourhood embedding (tsne) is used to visualise the low dimensional representation of the imaging data. the outputs of tsne are illustrated with 4 subplots, each created from different distance measurements. 
