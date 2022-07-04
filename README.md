# Yukun Zhou

I am a PhD student working with [Daniel C. Alexander](https://scholar.google.co.uk/citations?user=mH-ZOQEAAAAJ&hl=en) and [Pearse A. Keane](https://scholar.google.co.uk/citations?user=-7KS8pYAAAAJ&hl=en&oi=ao). I mainly work on medical image segmentation and model generalisability on large-scale dataset. I also enjoy the translational research, applying developed models on real-world clinical data. 

&nbsp;

# Project branches

* AutoMorph: automatic retinal vessel segmentation and morphology quantification
* Multi-class retinal vessel segmentation
* Segmentation model generalisability 
* Diabetic retinopathy and macular edema diagnosis 
* AI in Dementia 


# AutoMorph 👀
--Code for [AutoMorph: Automated Retinal Vascular Morphology Quantification via a Deep Learning Pipeline](https://www.medrxiv.org/content/10.1101/2022.05.26.22274795v1.full.pdf).


Before starting, we summarise the features for three running ways:

* Google Colab (no commands/code, free gpu for 12 hours; data privacy concern)
* Configure environment on local/virtual machine (data privacy, code development; packages conflict in some machines)
* Docker image (data privacy, no need to set up environment; need some experience on docker)

:star::star::star: If you meet unsolved problems, feel free to open an issue or drop a message to yukun.zhou.19[at]ucl.ac.uk

&nbsp;

## Index

- [AutoMorph 👀](#AutoMorph-)
  - [Quickstart with Colab](#quickstart-with-colab)
  - [Install instruction for local/virtual machine](#install-instruction-for-local/virtual-machine)
    - [Requirements](#requirements)
    - [Miniconda installation](#miniconda-installation)
    - [Package installation](#package-installation)
    - [Running](#running)
  - [Docker usage](#docker-usage)
  - [Common Questions](#common-questions)
    - [Memory/ram error](#memory/ram-error)
    - [Invalid results](#invalid-results)
  - [Components](#components)
  - [Citation](#citation)

&nbsp;



## Quickstart with Colab

Use the Google Colab and a free Tesla T4 gpu

[Colab link](https://colab.research.google.com/drive/13Qh9umwRM1OMRiNLyILbpq3k9h55FjNZ?usp=sharing)

&nbsp;

## Install instruction for local/virtual machine

### Requirements

1. Linux operating system. For windows, install [MinGW-w64](https://www.mingw-w64.org/) for using commands below to set enviroment or [docker desktop](https://docs.docker.com/desktop/windows/install/) for [docker usage](#docker-usage)
2. Anaconda or miniconda installed (installation steps below).
3. python=3.6, cudatoolkit=11.0, torch=1.7, etc. (installation steps below)
4. GPU is essential.

&nbsp;

### Miniconda install

If you already have miniconda or anaconda installed, please skip this section and go for package installation.

Step 1: Enter the path you want to put the installation and download the installer
```sh
$ cd <path/>
$ wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

Step 2: install, there are a few selections during installation, just select 'yes'
```sh
$ bash Miniconda3-latest-Linux-x86_64.sh
```

Step 3: activate
```sh
$ source ~/.bashrc
```

Step 4: check the installation
```sh
$ conda -V
```

&nbsp;

### Package installation

Step 1: create virtual environment and activate it:
```sh
$ conda update conda
$ conda create -n automorph python=3.6 -y
$ conda activate automorph
```

Step 2: install pytorch 1.7 and cudatoolkit 11.0
```sh
$ conda install pytorch==1.7.0 torchvision==0.8.0 torchaudio==0.7.0 cudatoolkit=11.0 -c pytorch -y
```

Step 3: install other packages:
```sh
$ pip install -r requirement.txt
$ pip install efficientnet_pytorch
```

&nbsp;

### Running

Please remember to activate virtual environment before running.
```sh
$ conda activate automorph
$ git clone https://github.com/rmaphoh/AutoMorph.git
```

Put the images in folder 'images' and
```sh
$ sh run.sh
```


Please not that resolution_information.csv includes the resolution for image, i.e., size for each pixel. Please prepare it for the customised data in the same format.

&nbsp;

## Docker usage

We also provide environment docker image for those who meet problems in package installation and are familiar with docker.

First, clone the github to <path/of/AutoMorph, e.g., /home/AutoMorph> and put the images in AutoMorph/images
```sh
$ git clone https://github.com/rmaphoh/AutoMorph.git
```

Then, pull our [docker image](https://hub.docker.com/r/yukundocker/image_automorph) and run the tool.
```sh
$ docker pull yukundocker/image_automorph
$ docker run  -v <path/of/AutoMorph>:/root/AutoMorph -ti --runtime=nvidia -e NVIDIA_DRIVER_CAPABILITIES=compute,utility -e NVIDIA_VISIBLE_DEVICES=all yukundocker/image_automorph
$ source /root/set_up.sh
```


&nbsp;

## Common questions

### Memory/ram error

We use Tesla T4 (16Gb) and 32vCPUs (120Gb). When you meet memory/ram issue in running, try to decrease batch size:

* ./M1_Retinal_Image_quality_EyePACS/test_outside.sh -b=64 to smaller, e.g., 32 or 16.
* ./M2_Artery_vein/test_outside.sh --batch-size=8 to smaller
* ./M2_lwnet_disc_cup/test_outside.sh --batchsize=8 to smaller

&nbsp;

### Invalid results

In results, invalid values (e.g., optic disc segmentation failure) is indicated by -1.  


&nbsp;

## Components

1. Vessel segmentation [BF-Net](https://github.com/rmaphoh/Learning-AVSegmentation.git)

2. Image pre-processing [EyeQ](https://github.com/HzFu/EyeQ.git) 

3. Optic disc segmentation [lwnet](https://github.com/agaldran/lwnet.git)

4. Feature measurement [retipy](https://github.com/alevalv/retipy.git)


&nbsp;

## Citation

```
@article{zhou2022automorph,
  title={AutoMorph: Automated Retinal Vascular Morphology Quantification via a Deep Learning Pipeline},
  author={Zhou, Yukun and Wagner, Siegfried and Chia, Mark and Zhao, An and Xu, Moucheng and Struyven, Robbert and Alexander, Daniel and Keane, Pearse and others},
  journal={medRxiv},
  year={2022},
  publisher={Cold Spring Harbor Laboratory Press}
}
```

