[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/koldLight/music-data/master)

# Music data experiments

## How to launch the notebooks

### Binder (no local installation required)

The easiest way to run the notebooks is via Binder. Click [here](https://mybinder.org/v2/gh/koldLight/music-data/master) and you'll have the notebooks available in a ready environment.

### Local installation

Requires:

* Python 3.8
* pipenv
* jupyter

To install `pipenv` (if not already installed):

```
sudo -H pip install -U pipenv
```

To install `jupyter` (if not already installed):

```
sudo -H pip install -U jupyter
```

To create the virtual enviroment and install the dependencies, run:

```
pipenv install --dev
```

And to create a jupyter notebook linked to this virtual enviroment:

```
# Activate the virtual environment
pipenv shell

# Create the kernel
python -m ipykernel install --user --name='music-data'

# Exit the virtual environment shell
exit
```

Now you'll have in your `jupyter` enviroment a new kernel named `music-data`.

Finally, to run the notebooks:

```
pipenv run jupyter notebook notebooks
```
