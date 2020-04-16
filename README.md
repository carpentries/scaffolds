# Scaffolds

This repository contains links to online tools that will help learners follow
lessons if they are having technical difficulties installing required software.

| Lesson | JupyterHub | JupyterLab | RStudio (binder) | RStudio (cloud) |
|--------|-----------|--------|-----------|--------|
| SWC Python Inflammation | [![Click here to launch python-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-inflammation) | [![Click here to launch python-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-inflammation?urlpath=lab) | | |
| SWC Python Gapminder | [![Click here to launch python-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-gapminder) | [![Click here to launch python-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-gapminder?urlpath=lab) | | |
| SWC R Inflammation | | | [![Click here to launch r-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-r-novice-inflammation?urlpath=rstudio)| |
| SWC R Gapminder | | | [![Click here to launch r-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-r-novice-gapminder?urlpath=rstudio)| |
| DC Ecology R | | | | |
| DC Ecology Python | | | | |
| DC Social Sciences R (Python version is not official) | | | | |
| DC Geospatial (R only) | | | | |
| DC Genomics (non-R only) | | | | |

## How this works

This repository hosts this README file on the main (master) branch. All other
branches on this repository are independent and contain the required data files
and setup to run in either [RStudio Cloud][rstudio-cloud] or 
[My Binder][my-binder]. 

Each new branch is created with the following command pair to first create the
branch with no history and then remove all files. 

```sh
git checkout --orphan <branchname>
git rm --cached -r .
```

The project can then be set up for the learner with the data set in a `data/`
directory and the setup instructions inside of a hidden `.binder/` directory
according to these set up rules: https://mybinder.readthedocs.io/en/latest/howto/index.html


[rstudio-cloud]: https://rstudio.cloud
[my-binder]: https://mybinder.org

