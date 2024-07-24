[![PyPI](https://img.shields.io/badge/python-3.9-yellow.svg)]()
[![license](https://img.shields.io/github/license/LinkedEarth/PyleoclimPaper.svg)]()
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LinkedEarth/PyleoclimPaper/HEAD)
[![DOI](https://zenodo.org/badge/377329396.svg)](https://zenodo.org/badge/latestdoi/377329396)

# Reproducible workflows using the Pyleoclim package

We present three reproducible workflows as Jupyter Notebook using the [Pyleoclim software package](https://pyleoclim-util.readthedocs.io/en/master/) to serve as fully executable companions to the Pyleoclim [manuscript](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022PA004509). The paper was published in 2022. Since then, we have made improvements to the code base and have created a special package for the handling of [LiPD files](https://lipd.net), [`pylipd`](https://pylipd.readthedocs.io/en/latest/), which works smoothly with `Pyleoclim`. The latest release of these notebooks represent these changes. If you wish to see the notebooks that were originally published with the manuscript and the 0.9.4 version of `Pyleoclim`, see [this tag](https://github.com/LinkedEarth/PyleoclimPaper/tree/v0.4).

We used `Pyleoclim` for the following studies:
* Orbital Cycles contains a workflow describing spectral and wavelet analysis of a marine record convering the past 5 million years/
* MD Confrontation contains a notebook reproducing the study by [Zhu et al. (2019)](https://www.pnas.org/doi/abs/10.1073/pnas.1809959116) looking at how well climate models capture the continnum of global-average temperature variability. 
* CrystalCorrelations contains a notebook looking at the pitfall of correlations for paleoclimate study following the study by [Hu et al. (2017)](https://www.sciencedirect.com/science/article/abs/pii/S0012821X16306823). 

The notebooks are fully executable through MyBinder (click on the badge at the top of this read me). 

## Pyleoclim

[Pyleoclim](https://pyleoclim-util.readthedocs.io/en/master/) is a Python package geared towards timeseries analysis of time-uncertain data.

The package can (but do not necessarily have to) directly work with data in the Linked Paleo Data ([LiPD](https://lipd.net)) format through the [`pylipd`](https://pylipd.readthedocs.io/en/latest/). The advantage of working with that format is that the code contains automated data transformation, making working with paleoclimate data easier and faster.

## Requirements

v1.0 of the notebooks require v1.1.0 of Pyleoclim and associated requirements detailed in the `environment.yml` file. A built container is available on [Quay.io](https://quay.io/repository/linkedearth/pyleoclim?tab=tags):

`docker pull quay.io/linkedearth/pyleoclim:db17c5968506`

## License

All notebooks herein are provided under an [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license.

## Citation
We needn't tell you that making research tools accessible requires time and effort. If you find any of these resources useful and use them in your own research, please do us the kindness of one or more citations. Notebooks in this collection is registered on Zenodo, and associated with a digital object identifier (DOI).  A ready-to-use citation is provided on this GitHub repository in APA and BibTex (in the About section on the right panel, click on "Cite this repository"). If you use any of the standards (LiPD) or the software (Pyleoclim), please cite them as well. It will make us (and NSF!) very happy to hear that these investments spawned more research.

If you use any of the data on this repository, please cite the original authors of the study. 
