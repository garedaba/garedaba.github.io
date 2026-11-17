---
layout: default
title: About μBrain
section: micro-brain
header_title: "&mu;Brain"
header_url: /micro-brain/
header_description: a 3D volumetric reconstruction of the mid-gestation fetal brain
links:
  - title: "&larr; &mu;Brain home"
    url: /micro-brain/
  - title: View the Project on GitHub
    small: garedaba/micro-brain
    url: https://github.com/garedaba/micro-brain
  - title: Download the Data from Zenodo
    small: 3D volume, surfaces and microarray data
    url: https://doi.org/10.5281/zenodo.10622337
---

# Important information
**&mu;Brain remains subject to revision.**  

Built upon existing open-source data, the &mu;Brain atlas is a freely-available 3D volumetric model of the mid-fetal brain. 

Using serial Nissl-stained and anatomically-labelled sections of the prenatal brain (Ding et al., 2022), we performed automated image repair using a generative neural network model before aligning all sections into a common anatomical space, resulting in a 3D volume at 150&mu;m voxel resolution. 

![slice-to-slice alignment and 3D reconstruction of uBrain]({{ '/micro-brain/assets/images/reconstruction.png' | relative_url }})

The &mu;Brain volume is accompanied by a set of brain tissue labels (n=20) and surface models of the cortical plate surface. The cortical surface is further parcellated into a set of cytoarchitecturally-defined labels (n=29). To facilitate integration with fetal and neonatal neuroimaging studies, the cortical surfaces and parcellations have been aligned to the fetal and neonatal surface templates of the [Developing Human Connectome Project](https://gin.g-node.org/kcl_cdb/dhcp_fetal_brain_surface_atlas).

![uBrain atlas on dHCP cortical surface]({{ '/micro-brain/assets/images/surfaces.png' | relative_url }})

In addition, cortical areas are matched to normalised gene expression data from corresponding laser microdissection microarrays across multiple tissue zones in three additional prenatal specimens (Miller et al. 2014).

&mu;Brain is a three-dimensional, high resolution histological atlas of the human fetal brain, coupled with bulk tissue microarray data, sampled across 29 cortical regions and 5 transient tissue zones. It provides a 3D anatomical coordinate space to facilitate integrated imaging-transcriptomic analyses of the developing brain.

# Citing &mu;Brain
&mu;Brain was introduced in our study of [cortical expansion in the fetal brain]({{ '/micro-brain/cortical_expansion/' | relative_url }}). If you use &mu;Brain in your work, please cite:

Ball, G., Oldham, S., Kyriakopoulou, V., Williams, L.Z.J., Karolis, V., Price, A., Hutter, J., Seal, M.L., Alexander-Bloch, A., Hajnal, J.V., Edwards, A.D., Robinson, E.C. & Seidlitz, J. Molecular signatures of cortical expansion in the human foetal brain. *Nat. Commun.* 15, 9685 (2024). [doi:10.1038/s41467-024-54034-2](https://doi.org/10.1038/s41467-024-54034-2)


 
# Data descriptors
## Volumetric data
**&mu;Brain-volume.nii.gz**  
a 3D reconstruction of the cerebral hemisphere at 150&mu;m resolution  

**&mu;Brain-atlas-labels.nii.gz**  
corresponding brain tissue labels (n=20)  

**brain-tissue-labels.txt**  
look-up table for brain tissue labels  

## Surface data
**&mu;Brain.R.inner/outer.surf.gii**  
inner and outer cortical surfaces of the &mu;Brain volume  

**&mu;Brain.cortical-atlas.fetal36w-template.label.gii**  
&mu;Brain cortical atlas projected onto the dHCP template surface  

**cortical_labels.txt**  
look-up table for cortical atlas labels  

## Microarray data
**&mu;Brain-processed-lmd-data.v1.csv**  
LMD microarray data aligned to the &mu;Brain cortical atlas in long format. Each row contains normalised expression for a single observation. Each observation is identified by tissue (cortical plate, subplate, etc), cortical region in &mu;Brain, specimen and gene.

## Thalamic atlas
A 3D atlas of thalamic nuclei derived from &mu;Brain, aligned to the dHCP fetal and neonatal templates and matched to microarray data, is available separately on [Zenodo](https://zenodo.org/records/24151361). See [Prenatal thalamus]({{ '/micro-brain/prenatal_thalamus/' | relative_url }}).



## Data resources & references
Ding, S.-L. et al. Cellular resolution anatomical and molecular atlases for prenatal human brains. J. Comp. Neurol. 530, 6–503 (2022)  

Miller, J. A. et al. Transcriptional landscape of the prenatal human brain. Nature 508, 199–206 (2014)  

[BrainSpan atlas](https://www.brainspan.org/)

## Project funding
<img src="{{ '/micro-brain/assets/images/funders.jpg' | relative_url }}" width="400"/>


