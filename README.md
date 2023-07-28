# BEATS Software Repository (BEATS) #

## What is this repository ##
This repo implements git submodules technique to list these repos in one space: 
1. BEATSH5Writer -- BEATS experimental data writer
2. BETAS_DAQ_Support_IOC -- tomoscan & writer support IOC
3. BEATS_Dashboard -- BEATS dashboard that is used to control all scan modules
4. BEATS_tomoscan -- forked repo from tomoscan@APS
5. RPTrigServ -- Raspberry Pi based simple triggering system for PCO detector.
6. BEATS_recon -- [TomoPy](https://tomopy.readthedocs.io/en/latest/) reconstruction scripts, notebooks and examples for the [BEATS beamline](https://beats-sesame.eu/).
7. [TomoPy](https://tomopy.readthedocs.io/en/latest/) -- An open-source Python package for tomographic data processing and image reconstruction.

## Quick usage guide ##
This repo is sub-module based repo that includes all BEATS related repos in one place. 

- To add a new sub-repo to BEATS repo: 
``` 
git submodule add <BEATS_related_repo_url>
```
- Cloning a Repository with Submodules:
If you want to clone this repo with all sub-modules: 
```
git clone git@github.com:SESAME-Synchrotron/BEATS.git
cd BEATS
git submodule update --init --recursive
```
- Updating Submodules:
When you pull changes to your main repository that include updates to the submodules, you need to update the submodules as well. Use the following command:
```
git submodule update --remote
```
This command fetches and applies changes from the remote repository of each submodule.
