Branch `release-clm5.0-add-params`.

This branch contains modifications on some modules for our study on ensemble simulations with perturbed parameters in the Community Land Model v.5.0 (CLM5). The modification allows for easy manipulation of hard-coded parameters. The parameters in the **PhotosynthesisMod**, **LunaMod**, and **SoilHydrologyMod** were added to the CLM parameter file. Similarly, the soil hydraulic parameters in the **SoilStateInitTimeConstMod** were added in the surface data file.

# Parameter Extraction
The following modules and parameters were impacted in *biogeophys*:

1. **PhotosynthesisMod**
- Parameters: vcmaxha, jmaxha, tpuha, lmrha, lmrhd, tpu25ratio, and theta_cj

2. **LunaMod**
- Parameters: jmaxb0, wc2wjb0

3. **SoilHydrologyMod**
- Parameter: fff

4. **SoilStateInitTimeConstMod**
- Parameters: psis_sat, shape_param, thetas, and ks

Exacting these parameters impacted other modules in *main*:
- **pftconMod**
- **readParamsMod**

## Usage
1. Clone the repository
2. Modify the extracted parameters in the CLM parameter file as needed.
3. Rebuild the CLM model to apply changes

## Caution
If you are not interested in perturbing the soil hydraulic parameters in **SoilStateInitTimeConstMod**, use the default module. 


# CTSM

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3739617.svg)](https://doi.org/10.5281/zenodo.3739617)

## Overview and resources

The Community Terrestrial Systems Model.

This includes the Community Land Model (CLM5.0 and CLM4.5) of the Community Earth System Model.

For documentation, quick start, diagnostics, model output and
references, see

http://www.cesm.ucar.edu/models/cesm2.0/land/

and

https://escomp.github.io/ctsm-docs/

For help with how to work with CTSM in git, see

https://github.com/ESCOMP/CTSM/wiki/Quick-start-to-CTSM-development-with-git

and

https://github.com/ESCOMP/ctsm/wiki/Recommended-git-setup

For support with model use, troubleshooting, etc., please use the CTSM forum (or other
appropriate forum) here:

https://xenforo.cgd.ucar.edu/cesm/

To get updates on CTSM tags and important notes on CTSM developments
join our low traffic email list:

https://groups.google.com/a/ucar.edu/forum/#!forum/ctsm-dev

(Send email to ctsm-software@ucar.edu if you have problems with any of this)

## CTSM code management team

CTSM code management is provided primarily by:

Software engineering team:
- [Erik Kluzek](https://github.com/ekluzek)
- [Bill Sacks](https://github.com/billsacks)
- [Mariana Vertenstein](https://github.com/mvertens)
- [Negin Sobhani](https://github.com/negin513)
- [Sam Levis](https://github.com/slevisconsulting)

Science team:
- [Dave Lawrence](https://github.com/dlawrenncar)
- [Will Wieder](https://github.com/wwieder)
- [Danica Lombardozzi](https://github.com/danicalombardozzi)
- [Keith Oleson](https://github.com/olyson)
- [Sean Swenson](https://github.com/swensosc)
- [Mike Barlage](https://github.com/barlage)
- [Rosie Fisher](https://github.com/rosiealice)
- [Peter Lawrence](https://github.com/lawrencepj1)
