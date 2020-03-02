# phy: interactive visualization and manual spike sorting of large-scale ephys data

[![Build Status](https://travis-ci.org/cortex-lab/phy.svg)](https://travis-ci.org/cortex-lab/phy)
[![codecov.io](https://img.shields.io/codecov/c/github/cortex-lab/phy.svg)](http://codecov.io/github/cortex-lab/phy)
[![Documentation Status](https://readthedocs.org/projects/phy/badge/?version=latest)](https://phy.readthedocs.io/en/latest/?badge=latest)
[![GitHub release](https://img.shields.io/github/release/cortex-lab/phy.svg)](https://github.com/cortex-lab/phy/releases/latest)
[![PyPI release](https://img.shields.io/pypi/v/phy.svg)](https://pypi.python.org/pypi/phy)


[**phy**](https://github.com/cortex-lab/phy) is an open-source Python library providing a graphical user interface for visualization and manual curation of large-scale electrophysiological data. It is optimized for high-density multielectrode arrays containing hundreds to thousands of recording sites (mostly [Neuropixels probes](https://www.ucl.ac.uk/neuropixels/)).

[![phy 2.0b1 screenshot](https://user-images.githubusercontent.com/1942359/74028054-c284b880-49a9-11ea-8815-1b7e727a8644.png)](https://user-images.githubusercontent.com/1942359/74028054-c284b880-49a9-11ea-8815-1b7e727a8644.png)


## What's new

* [7 Feb 2020] Release of phy 2.0 beta 1, with many new views, new features, various improvements and bug fixes...


## Links

* [Documentation](http://phy.readthedocs.org/en/latest/)
* [Mailing list](https://groups.google.com/forum/#!forum/phy-users)


## Installation instructions

Phy requires a recent GPU and an SSD for storing your data (the GUI may be slow if the data is on an HDD).

1. Install the latest version of [Anaconda 64-bit with Python 3](https://www.anaconda.com/distribution/#download-section).

2. Open a terminal and type:

```bash
conda create -n phy2 python pip numpy matplotlib scipy sklearn h5py pyqt cython pillow -y
conda activate phy2
pip install phy
```

3. Phy should now be installed. Open the GUI on a dataset as follows (the phy2 environment should still be activated):

```bash
cd path/to/my/spikesorting/output
phy template-gui params.py
```


### Upgrading from phy 1 to phy 2

* Do not install phy 1 and phy 2 in the same conda environment.
* It is recommended to delete `~/.phy/*GUI/state.json` when upgrading.


### Developer instructions

To install the development version of phy in a fresh environment, do:

```bash
git clone https://github.com/cortex-lab/phy.git
cd phy
pip install -r requirements.txt
pip install -r requirements-dev.txt
pip install -e .
```

### Troubleshooting

* [Raise a GitHub issue.](https://github.com/cortex-lab/phy/issues)


## Credits

**phy** is developed and maintained by [Cyrille Rossant](http://cyrille.rossant.net).

* [International Brain Laboratory](https://internationalbrainlab.org)
* [Cortex Lab (UCL)](https://www.ucl.ac.uk/cortexlab/) ([Kenneth Harris](https://www.ucl.ac.uk/biosciences/people/harris-kenneth) and [Matteo Carandini](https://www.carandinilab.net/)).

Contributors to the repository are:

* [Alessio Buccino](https://github.com/alejoe91)
* [Michael Economo](https://github.com/mswallac)
* [Cedric Gestes](https://github.com/cgestes)
* [Dan Goodman](http://thesamovar.net/)
* [Max Hunter](https://iris.ucl.ac.uk/iris/browse/profile?upi=MLDHU99)
* [Shabnam Kadir](https://iris.ucl.ac.uk/iris/browse/profile?upi=SKADI56)
* [Christopher Nolan](https://github.com/crnolan)
* [Martin Spacek](http://mspacek.github.io/)
* [Nick Steinmetz](http://www.nicksteinmetz.com/)
