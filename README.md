## Welcome to PRIME-RE
### The PRIMatE Research Exchange

The preprocessing and analysis of nonhuman primate (NHP) magnetic resonance imaging (MRI) data presents some unique challenges. Over the years, many laboratories and researchers have created their own custom solutions to many of these problems. PRIME-RE aims to provide a overview of the main difficulties and curate a collection of solutions that currently exist within the broader NHP-MRI communnity for specific processing steps that are commonly performed on NHP MRI data. Since this is a cimmunity effort, we strongly encourage you to contribute your workflows and pipelines. 

PRIME-RE is maintained by members of the [PRIME-DE consortium](http://fcon_1000.projects.nitrc.org/indi/indiPRIME.html). 

![logo](images/social_preview_image.png)

#### How to contribute ?
Send new content by using [this template file](New_Resource_Template.md) to create a new issue [here](https://github.com/PRIME-RE/prime-re.github.io/issues)! You can also join our communication channel around the Primate Data Exchange on the Brainhack community on [PRIME-DE Mattermost-channel](https://mattermost.brainhack.org/brainhack/channels/prime-de) or specifically for this Primate Resource Exchange via on [PRIME-RE Mattermost-channel](https://mattermost.brainhack.org/brainhack/channels/prime-re) .

#### Wiki
A [wiki](https://github.com/PRIME-RE/prime-re.github.io/wiki/Structural-preprocessing) have been set up to share knowledge about NHP MRI acquisition and image processing. Anyone can share knowledge and experience (problems with solutions, fixes, tricks...).

### [Atlases](#atlases)

### [Structural preprocessing](#structpreproc)
  
  - [What is it about?](#structdescription)
  - [Issues linked to NHP imaging](#structissues)
  - [Steps](#structsteps)
      - [Preparation of data (Cropping, deoblique…)](#structpreparation)
      - [Registration to template](#structregistration)
      - [Brain extraction / skull stripping](#structextraction)
      - [Segmentation (GM, WM, CSF? Subcortical?bone, non brain soft tissue? air?)](#structsegmentation)
      - [Surface generation](#structsurf)
      - [Morphometry measures (thickness, curvature etc)](#structmeasures)
      
  - [Pipelines Reviews](#structlinks)  
  - [Communication](structural_preprocessing/data_preparation.md#communication)
   

### [fMRI preprocessing](#funcpreproc)


<a name="atlases"></a>
# Atlases
Comming soon...

<a name="structpreproc"></a> 
# Structural preprocessing
<a name="structlinks"></a> 
## Pipelines Reviews
### Chris' notebook
(description should be here)
[Chris' notebook html](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html)  - [Download Chris' notebook](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb)
### Macapype
Python package that provides pipelines for NHP anatomical preprocessing using Nipype.
[framagit repository](https://framagit.org/mars-hackat2019/anat-mri-pipeline/macapype)

| Name | Short description | Links |
| --- | --- | --- |
| Surfaces and flatmaps | Jupyter notebook that ... | [view](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.html) - [download](structural_preprocessing/surfaces_and_flatmaps_notebook/Surfaces_and_Flatmaps.ipynb) |
| Macapype | Python package for anatomical preprosessing using Nipype. | [github](https://framagit.org/mars-hackat2019/anat-mri-pipeline/macapype) - [details](https://github.com/PRIME-RE/prime-re.github.io/issues/7) |

<a name="funcpreproc">
# Functional Preprocessing
 To be continued...









