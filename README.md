# project_SHEBA
This repository contains code used to reproduce analysis for the paper. The notebooks are available in read format. In order to re-run the code, the user must download the trajectory data used in this study and the IGRA dataset v2

## Cloudy state profiles
All_cloudy_profiles_v_28_10_2019.ipynb file contains the figures used to show cloudy state analysis

## Clear state profiles
all_clear_profiles_v31_10_2019.ipynb file contains the figures used for clear state analysis

## Important python files
* traj_check.py checks if a given trajectory is passing through a observation station. *Prerequiste: Path to IGR_25N_v2.xlsx file to function*

* sounding_finder.py reads IGRA data-set from a particular station and for a particular date and returns it as a Pandas dataframe. *Prerequiste: In the code change the path to dir where IGRA dataset is stored before using.* 
