# AMASS: Archive of Motion Capture as Surface Shapes

![alt text](github_data/datasets_preview.png "Samples of bodies in AMASS recovered from Motion Capture sequences")

[AMASS](http://amass.is.tue.mpg.de) is a large database of human motion unifying different optical marker-based motion capture datasets by representing them within a common framework and parameterization. 
 AMASS is readily useful for animation, visualization, and generating training data for deep learning.

Here we provide tools and tutorials to use AMASS in your research projects. More specifically:
- Following the recommended splits of data by AMASS, we provide three non-overlapping train/validation/test splits.
- AMASS uses an extended version of [SMPL+H](http://mano.is.tue.mpg.de/) with [DMPLs](http://smpl.is.tue.mpg.de/downloads). 
Here we show how to load different components and visualize a body model with AMASS data.
- AMASS is also compatible with [SMPL](http://smpl.is.tue.mpg.de) and [SMPL-X](https://smpl-x.is.tue.mpg.de/) body models. 
We show how to use the body data from AMASS to animate these models.
## Table of Contents
  * [Installation](#installation)
  * [Body Models](#body-models)
  * [Tutorials](#tutorials)
  * [Citation](#citation)
  * [License](#license)
  * [Contact](#contact)

## Installation
**Requirements**
- Python 3.7
- [Human Body Prior](https://github.com/nghorbani/human_body_prior)
- [Pyrender](https://pyrender.readthedocs.io/en/latest/install/index.html#osmesa) for visualizations

Install from this repository for the latest developments:
```bash
pip install git+https://github.com/lsteiner91/configer
pip install git+https://github.com/lsteiner91/human_body_prior
pip install git+https://github.com/lsteiner91/amass
```

## Body Models
AMASS fits a statistical body model to labeled marker-based optical motion capture data.
In the paper originally we use [SMPL+H](http://mano.is.tue.mpg.de/downloads) with extended shape space, e.g. 16 betas, and 
[DMPLs](http://smpl.is.tue.mpg.de/downloads). 
Please download each and put them in body_models folder of this repository after you obtained the code from GitHub.

## Tutorials
We release tools and multiple Jupyter notebooks to demonstrate how to use AMASS to animate SMPLH body model.

Furthermore, as promised in the supplementary material of the paper, we release code to produce synthetic mocap using 
[DFaust](http://dfaust.is.tue.mpg.de) registrations.

Please refer to [tutorials](/notebooks) for further details.

## Citation
Please cite the following paper if you use this code directly or indirectly in your research/projects:
```
@inproceedings{AMASS:2019,
  title={AMASS: Archive of Motion Capture as Surface Shapes},
  author={Mahmood, Naureen and Ghorbani, Nima and F. Troje, Nikolaus and Pons-Moll, Gerard and Black, Michael J.},
  booktitle = {The IEEE International Conference on Computer Vision (ICCV)},
  year={2019},
  month = {Oct},
  url = {https://amass.is.tue.mpg.de},
  month_numeric = {10}
}
```
## License

Software Copyright License for **non-commercial scientific research purposes**.
Please read carefully the [terms and conditions](./LICENSE) 
and any accompanying documentation before you download and/or use the AMASS dataset, and software, (the "Model & Software"). 
 By downloading and/or using the Model & Software 
 (including downloading, cloning, installing, and any other use of this GitHub repository), 
 you acknowledge that you have read these terms and conditions, understand them, 
 and agree to be bound by them. If you do not agree with these terms and conditions, 
 you must not download and/or use the Model & Software.
  Any infringement of the terms of this agreement will automatically terminate your rights under this [License](./LICENSE).
 
 ## Contact
The code in this repository is developed by [Nima Ghorbani](https://nghorbani.github.io/).

If you have any questions you can contact us at [amass@tuebingen.mpg.de](mailto:amass@tuebingen.mpg.de).

For commercial licensing, contact [ps-licensing@tue.mpg.de](mailto:ps-licensing@tue.mpg.de)
