## Nilearn

| Viewing 3D MR brain image |
|:---:|
| [![T1 weighted](demos/mni.jpg "MNI template")](demos/mni.html)|


| Correlation matrix on a glass brain |
|:---:|
| [![rsfMRI](demos/conn.png "Correlation on 39 regions")](demos/connectome.html)|


| Regions as markers on a glass brain |
|:---:|
| [![rsfMRI](demos/markers.png "Markers: 39 regions")](demos/markers.html)|

## FSLEyes - Harvard Oxford Atlas


    fsleyes /usr/local/fsl/data/atlases/HarvardOxford/HarvardOxford-cort-maxprob-thr25-2mm.nii.gz

## MRtrix3 - Tractogram visualization

    mrview dwi_den_preproc_unbiased.mif -tractography.load smallerTracks_200k.tck