# openmc_fusion_tutorial

This is a step-by-step to getting openmc (hopefully) easily.

## 1. Get Micromamba
`Micromamba` is a Python package-management system. It's similar to `Anaconda` (or `conda`), but it's faster, and in my opinion, just a better experience.

[This link](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html) has the instructions to download and install micromamba.

## 2. Use Micromamba to install openmc
Luckily, [OpenMC](https://github.com/openmc-dev/openmc) is nicely packaged and deployed, so there's no need to build anything, or mess with Git. Using micromamba, do:

```
[path_to_micromamba] install openmc -c conda-forge
```

** Note if you have a Mac with M chips, it might not work. If that's the case, try [this approach to create an intel conda environment](https://blog.rtwilson.com/how-to-create-an-x64-intel-conda-environment-on-your-apple-silicon-mac-arm-conda-install/) and then installing `openmc` after.

## 3. Test openmc
Example OpenMC input files [here](https://github.com/openmc-dev/openmc/tree/develop/examples). Two ways of running OpenMC:
- Run a python script using the OpenMC Python API (recommended)
- construct the XML input files, and run `openmc` executable on the directory

## 4. Other helpful links
- This is a [great fusion neutronics workshop](https://github.com/fusion-energy/neutronics-workshop) by Jonathan Shimwell. Mostly everything by Jon is great.
