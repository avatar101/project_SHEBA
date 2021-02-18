# Project SHEBA
This repository contains code used to reproduce figures for the Paper:[Following moist intrusions into the Arctic using SHEBA observations in a Lagrangian perspective](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.3859). The notebooks are also available in read format and can be viewed here on GitHub.

# Set Up
* In order to re-run the code, the user must download the [trajectory data](https://doi.pangaea.de/10.1594/PANGAEA.899851?format=html#download) used in this study, the [IGRA dataset version2](https://data.nodc.noaa.gov/cgi-bin/iso?id=gov.noaa.ncdc:C00975) and the [SHEBA radiosonde data](https://data.eol.ucar.edu/dataset/13.202) and change the path to these datasets accordingly in the code.
* Before proceeding further install `anaconda` if it isn't already installed. Users can also install `miniconda` if they don't want to install all the packages that comes with anaconda.
* On the termial execute `conda env create -f work_environment_journal.yml` to install the packages used in this study from work_environment_journal.yml provided here. 

## Cloudy vs Clear state trajectories

[Traj_cloudy_vs_clear_v_journal.ipynb](https://github.com/avatar101/project_SHEBA/blob/master/Traj_cloudy_vs_clear_v_journal.ipynb) file contains the figure used to compare all the trajectories for clear vs cloudy states.

## Cloudy state profiles
[All_cloudy_profiles](https://github.com/avatar101/project_SHEBA/blob/master/All_cloudy_profiles_v_journal.ipynb) file contains the figures used to show cloudy state analysis

## Clear state profiles
[all_clear_profiles](https://github.com/avatar101/project_SHEBA/blob/master/All_clear_profiles_v_journal.ipynb) file contains the figures used for clear state analysis

## Forward trajectory profile
[Plot_forward_journal2.ipynb](https://github.com/avatar101/project_SHEBA/blob/master/Plot_forward_journal2.ipynb) contains the figures used for forward trajectory analysis

## Important modules
* [traj_check.py](https://github.com/avatar101/project_SHEBA/blob/master/traj_check.py) checks if a given trajectory is passing through a given observation station. *Prerequiste: Path to IGR_25N_v2.xlsx file to function*

* [sounding_finder.py](https://github.com/avatar101/project_SHEBA/blob/master/sounding_finder.py) reads IGRA data-set from a particular station and for a particular date and returns it as a Pandas dataframe. *Prerequiste: It requires the user to first download the IGRA v2 dataset separately. In this function change the path (line 31 and line 75) to dir where IGRA dataset is stored before using.* 
