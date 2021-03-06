
---

##### [Template/Atlas](templates_and_atlases.md) &nbsp;  - &nbsp;  [General](pipelines_general.md) &nbsp;  - &nbsp;  [Structural](pipelines_structural.md) &nbsp;  - &nbsp;  [fMRI](pipelines_fmri.md) &nbsp;  - &nbsp;  [Diffusion](pipelines_diffusion.md) &nbsp;  - &nbsp;  [Data](data_sharing.md) &nbsp;  - &nbsp; [Software packages](software_packages.md)  &nbsp;  - &nbsp; [Hardware](hardware.md)          
---    

# Templates and atlases

Jump to:
- [macaque](templates_and_atlases_macaque.md)
- [marmoset](templates_and_atlases_marmoset.md)  

<br>   


## Details

**Template:** A standard brain, typically used for registering multiple individuals into a common coordinate space. This space can be either volumetric (3D coordinates system), surface-based (mesh), or a combination of both.

**Atlas:** a percellation of the brain into areas, often provided in a specific template space. Atlases are typically used for defining regions-of-interest (ROIs) or for identifying the location of activation sites.

For human MRI, the [MNI template](http://www.bic.mni.mcgill.ca/ServicesAtlases/ICBM152NLin2009) serves as the community standard volumetric template. Its integration into most major software packages makes it easy for researchers to register their results to MNI space. This facilitates data-sharing, cross-study comparisons and metanalyses. Most human brain atlases are also provided in MNI space. For surface-based analysis the [FsAverage](https://surfer.nmr.mgh.harvard.edu/fswiki/FsAverage) (freesurfer average) template serves the same purpose.

When it comes to NHP neuroimaging though, there are two complications:
1. The usage of multiple species creates the need for species-specific templates
2. Even for the most commonly imaged species (macaques and marmosets), multiple templates are available, with no single one of them adopted as the go-to community standard.

Below, we provide a non-exhaustive list of existing templates and atlases. For a more detailed resource list of templates and atlases see [this list for macaques](templates_and_atlases_macaque.md) or [here for marmosets](templates_and_atlases_marmoset.md).


<br>   

<a name="macaque_atlases"></a>
## Macaque

| Template | Species | Resolution (mm<sup>3</sup>) | With atlas | Volume format | Surface format | Links |
| --- | --- | --- | --- | --- | --- | --- |
| NMT | _M. mulatta_ | 0.25 | Saleem Logothetis (D99-SL) | NIFTI | GIFTI | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5660669/) [download](https://github.com/jms290/NMT) |
| D99 | _M. mulatta_ | 0.25 | D99-SL | NIFTI | GIFTI | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6075609/) [download](https://afni.nimh.nih.gov/Macaque) |
| INIA19 | _M. mulatta_ | 0.50 | Neuromaps | NIFTI | N/A | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3515865/) [download](https://www.nitrc.org/projects/inia19/https://www.nitrc.org/projects/inia19/) |
| MNI macaque | _M. fascicularis_ & _M. mulatta_ | 0.25 | Paxinos | MINC & NIFTI | N/A | [reference](https://www.ncbi.nlm.nih.gov/pubmed/21256229) [download](http://www.bic.mni.mcgill.ca/ServicesAtlases/Macaque) |
| Yerkes19 | _M. mulatta_ | 0.50 | F99 | NIFTI & MGZ | GIFTI & MGZ | [reference1](https://www.pnas.org/content/115/22/E5183) [reference2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3500860/) [download1](https://balsa.wustl.edu/reference/show/976nz) [download2](https://github.com/Washington-University/NHPPipelines) |
| Japanese macaque atlas| _M. fuscata_ | 0.50 | N/A | ANALYZE | N/A | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3221050/) [download](https://brainatlas.brain.riken.jp/jm/modules/xoonips/listitem.php?index_id=9) |
| 112RM-SL | _M. mulatta_ | 0.50 | D99-SL & F99 | NIFTI | N/A | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2659879/) |
| UNC-Emory developmental atlas | _M. mulatta_ | 0.60 | multiple | NRRD | N/A | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5222830//) [download](https://www.nitrc.org/projects/macaque_atlas/) |

For a more detailed resource list of macaque templates and atlases see [this list](templates_and_atlases_macaque.md).

<a name="macaque_warps"></a>
### Warps between macaque templates
Transforming data (e.g. parcellations, statistical maps) between the various template spaces requires the registration of those templates to one another. The [RheMAP](templates_and_atlases/rhemap.md) package provides pre-calculated warps between a set of common rhesus macaque brain templates. These warps can be directly downloaded from [Zenodo](https://doi.org/10.5281/zenodo.3668510
). Corresponding code is available on [GitHub](https://github.com/PRIME-RE/RheMAP).     

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3668510.svg)](https://doi.org/10.5281/zenodo.3668510)

<br>   

<a name="marmoset_atlases"></a>
## Marmoset

| Template | Species | Resolution (mm<sup>3</sup>) | With atlas | Volume format | Surface format | Links |
| --- | --- | --- | --- | --- | --- | --- |
| NIH | _C. jacchus_ | 0.15 | NIH (3 parcellations) | NIFTI | CARET | [reference](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5856608/) [download1](https://www.nitrc.org/projects/nih_marmoset/)  [download2](https://github.com/cirongliu/NIH_Marmoset_Atlas_V1) |
| RIKEN | _C. jacchus_ | 0.2 | N/A | NIFTI | N/A | [reference](https://www.sciencedirect.com/science/article/abs/pii/S1053811910013546?via%3Dihub) [download](https://brainatlas.brain.riken.jp/marmoset/modules/xoonips/detail.php?id=004) |
| 3D Paxinos et al. (2012) | _C. jacchus_ | 0.04×0.5×0.04 | Cortical areas of the Paxinos et al., (2012) | NIFTI | N/A | [reference](http://www.marmosetbrain.org/reference) |     
| Nencki-Monash | _C. jacchus_ | 0.05 | Cortical areas of the Paxinos et al., (2012) | NIFTI | N/A | [reference](http://www.marmosetbrain.org/nencki_monash_template) |   

For a more detailed resource list of marmoset templates and atlases see [this list](templates_and_atlases_marmoset.md).

<br>   

<a name="other_atlases"></a>
## Other species

| Template | Species | Resolution (mm<sup>3</sup>) | With atlas | Volume format | Surface format | Links |
| --- | --- | --- | --- | --- | --- | --- |
| Mouse Lemur atlas | _Microcebus murinus_ | 0.091 | YES | NIFTI | N/A | [reference](https://www.sciencedirect.com/science/article/abs/pii/S1053811918319694?via%3Dihub) [download](https://www.nitrc.org/projects/mouselemuratlas) |
