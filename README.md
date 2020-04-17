# Scaffolds

This repository contains links to online tools that will help learners follow
lessons if they are having technical difficulties installing required software.

| Lesson | JupyterHub | JupyterLab | RStudio (binder) | RStudio (cloud) |
|--------|-----------|--------|-----------|--------|
| SWC Python Inflammation | [![Click here to launch python-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-inflammation) | [![Click here to launch python-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-inflammation?urlpath=lab) | | |
| SWC Python Gapminder | [![Click here to launch python-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-gapminder) | [![Click here to launch python-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-gapminder?urlpath=lab) | | |
| SWC R Inflammation | | | [![Click here to launch r-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-r-novice-inflammation?urlpath=rstudio)| [swc-r-novice-inflammation in RStudio Cloud](https://rstudio.cloud/project/1167299) |
| SWC R Gapminder | | | [![Click here to launch r-novice-gapminder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-r-novice-gapminder?urlpath=rstudio)| [swc-r-novice-gapminder in RStudio Cloud](https://rstudio.cloud/project/1151792) |
| DC Ecology R | | | [![Click here to launch ecology-r](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-ecology-r?urlpath=rstudio)| [dc-ecology-r in RStudio Cloud](https://rstudio.cloud/project/1167280) |
| DC Ecology Python | [![Click here to launch dc-ecology-python JupyterHub](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-ecology-python) | [![Click here to launch dc-ecology-python JupyterLab](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-ecology-python?urlpath=lab) | | |
| DC Social Sciences R (Python version is not official) | | | [![Click here to launch dc-social-science-r RStudio](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-social-science-r?urlpath=rstudio) | [dc-social-science in RStudio Cloud](https://rstudio.cloud/project/1167422) |
| DC Geospatial (R only) | | | [![Click here to launch dc-geospatial-r RStudio](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-geospatial-r?urlpath=rstudio) | [dc-geospatial-r in RStudio Cloud](https://rstudio.cloud/project/1167320)|
| DC Genomics (non-R only) | | | <!-- NOT YET AVAILABLE [![Click here to launch dc-genomics RStudio](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/dc-genomics?urlpath=rstudio) --> | |

# Guide to Resources

These resources provide instances of python, R, and bash without the learner needing to install software. 

## Binder (https://mybinder.net)

This resource comes with everything pre-configured and will open in one of the
JupyterHub, JupyterLab, or RStudio interfaces. There are limitations to this
approach:

 - startup can take anywhere from 30 seconds to 30 minutes, depending on when
   it was last built
 - sessions expire with 10 minutes of inactivity
 - data does not persist between sessions
 - limited to 100 simultaneous users per session

The benefits for this is that there is no log in for users and it works
directly in the browser.

## RStudio Cloud (https://rstudio.cloud)

This resource is exclusively for R-based lessons. It requires a login from
users, either through Google, GitHub, or on-site registration. The templates 
were created by hand and are not explicitly synched with this repository. 

--------------------------------------------------------------------------------

# How this repository works

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

