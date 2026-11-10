# CAMELS-MX 

## Quality control of streamflow data

### Key items to measure 

1. All values are positive (i.e., all negative values are replaced by nan (np.nan))
2. if there are hourly and daily timeseries, they must match.
3. identify flatline data
4. identify potential outliers by identify min and max, and values more than 1, 2 and 3 std deviation from the mean
5. Identify duplicate dates

### Key items to do:
1. Plot of timeseries (entire timeseries, seasonality, sub-daily, exceedance curve)
2. compute how many nans are per timeseries 
3. Keep any flags from data (was performed in camels-de, camels-uk (even with remsapling))
4. normalize column names (if needed)

### References. 

1. CAMELS-DE: https://camels-de.org/camels_de/
https://github.com/CAMELS-DE/camels_de/blob/v1.0.0/version1/scripts/00_fix_errors_in_data.ipynb






# Python ENV
## Create virtual environment
pyenv virtualenv 3.11.9 camels_mx_qc

## Activate environment
pyenv activate camels_mx_qc

## Install packages
python -m pip install pandas numpy matplotlib scipy fastparquet


pip list
Package                 Version
----------------------- --------
appnope                 1.0.0
asttokens               3.0.2
comm                    0.2.3
contourpy               1.3.3
cramjam                 2.14.0
cycler                  0.12.1
debugpy                 1.8.22
executing               2.3.0
fastparquet             2026.9.0
fonttools               4.68.0
fsspec                  2026.9.0
ipykernel               7.4.0
ipython                 9.18.1
ipython_pygments_lexers 1.1.1
jedi                    0.20.1
jupyter_client          8.10.0
jupyter_core            5.9.1
kiwisolver              1.5.1
matplotlib              3.11.2
matplotlib-inline       0.2.2
nest-asyncio2           1.7.4
numpy                   2.4.6
packaging               26.3
pandas                  3.1.1
parso                   0.8.7
pexpect                 4.9.0
pillow                  13.0.0
pip                     24.0
platformdirs            4.14.5
prompt_toolkit          3.0.53
psutil                  7.2.2
ptyprocess              0.7.0
pure_eval               0.2.4
Pygments                2.21.0
pyparsing               3.3.3
python-dateutil         4.0.0
pyzmq                   27.3.0
scipy                   1.17.1
setuptools              65.5.0
stack-data              0.6.3
tornado                 6.6.1
traitlets               5.16.1
typing_extensions       4.16.0
tzdata                  2026.6
wcwidth                 0.9.4