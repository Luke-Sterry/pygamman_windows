# pygamman_windows
Step by step guide on how to compile the pygamman function for windows users using WSL (Ubunutu) and miniconda

## Prerequisites
1. Install WSL:
   Open Powershell and run:
   wsl --install

2. pip install jupyter
3. pip install setuptools
4. Install miniconda

## Versions used
Miniconda
Jupyter
WSL
python


(This code worked on Python 3.11.14 so upgrade/downgrade accoridngly)

## Downloading pygamman
Download the "pygamman_f2py-master" folder from https://github.com/guidov/pygamman_f2py

If repeating this step, delete any existing “pygamman_f2py-master” folder and redownload the “pygamman_f2py-master folder and save it in the same directory location as the 1_ and 2_.py files (for Broullón et al. 2026 method)

## Ubuntu Coding
In Ubuntu, copy and paste:
git clone https://github.com/Luke-Sterry/pygamman_windows.git
cd pygamman_windows

### Create the Environment
Copy and paste this into Ubuntu:
conda env create -f environment.yml
conda activate pygamman_windows_env
(will take a few minutes so be patient)

Check it's installed by typing: conda env list

### Activate Environment
conda activate pygamman_windows_env

## Navigate to pygamman folder
cd "/mnt/c/Users/sterr/OneDrive - University of Southampton/PhD/Espe Code/pygamman_f2py-master"

# Compiling pygamman
Type:
make clean
make




