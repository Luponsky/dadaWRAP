# dadaWRAP

# install miniconda
```
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh


# We need to interact with the following during installation:

 # We will be asked to review the licence agreement. After pressing return/enter, we can view it and hit the space bar to advance. At the bottom, we need to type in yes to accept.
 # It will then ask if the location is ok, hitting enter will place it in our current home directory, which is usually great.
 # At the end it will ask if we want to update our shell profile to automatically initialize conda.
 # There might be reasons to not want to do this, but until we hit one of those reasons, for most users it’s easist just to say yes to that.


bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm -rf ~/miniconda3/miniconda.sh

source ~/.bash_profile || source ~/.bashrc


# install mamba

conda install -n base -c conda-forge mamba


```




 

## installation with conda/mamba

```
conda create -n dadaWRAP  
conda activate dadaWRAP
mamba env update -n dadaWRAP --file dadawrapp.yaml
```
mamba install figaro

./dadaWRAP.0.3.sh -i datiseq/ -a GTGYCAGCMGCCGCGGTAA -A CCGYCAATTYMTTTRAGTTT  -cutap -figaro  -l 372

