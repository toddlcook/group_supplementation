# Probabilistic Group Supplementation

### Introduction
This repo is for the code used in Chapters 3 and 4 of my [thesis](https://drive.google.com/file/d/1UHI1Lv3xPMNuvpRDa3q7VkXNhoXUD-P1/view).


The two chapters describe my method in probabilistically appending photometric galaxies to spectroscopically confirmed galaxy groups.
This is done in the effort to better retrieve properties of the dark matter haloes in which the groups lie.

The data used for these notebooks can be found in this [Google Drive](https://drive.google.com/drive/folders/1FtsA5wm-F9Xvzk5hVvTK1ms08UHbgyR0?usp=sharing).

This is **excluding** the p(z) posteriors for photometric galaxies in the GAMA regions produced by TOPz. 

The **G09 posteriors** can be found in the Apollo2 Lustre space at ```/mnt/lustre/projects/astro/general/tc339/g09_posteriors```.

The **G12** and **G15 posteriors** can be found ```/mnt/lustre/projects/astro/general/tc339/GAMA_supplementation/g12_g15_posteriors```.

It's important you **don't open** these folders in a broswer for example because there are thousands of files in there. Access each individual posterior through Python instead.


### Notebooks
In **Euclid_photo_groups.ipynb**, we establish the profile of haloes used for subsequent notebooks, and test out our photometric supplementation method on simulated data (Euclid FS2 simulation)

In **GAMA_supplementation.ipynb**, we apply our supplementation method to GAMA, using spectroscopically confirmed GAMA groups and photometric galaxies with a photo-z posterior using TOPz.

In **GAMA_supplementation_HMF.ipynb**, we use our newly derived halo masses to emperically calculate the Halo Mass Function from GAMA groups.

**GAMA_supplementation_HMF_mean.ipynb** is a duplicate of the former notebook, but instead using the geometric mean of our supplemented luminosity mass and the dynamical mass.

![HMF mean](https://github.com/toddlcook/group_supplementation/blob/main/plots/HMF_mean.jpg)
