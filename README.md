# Scaffolds

This repository contains links to online tools that will help learners follow
lessons if they are having technical difficulties installing required software.

| Lesson | Resources |
|--------|-----------|
| SWC Python Inflammation|[![Click here to launch python-novice-inflammation](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/carpentries/scaffolds/swc-python-novice-inflammation)|
| SWC Python Gapminder||
| SWC R Inflammation||
| SWC R Gapminder||
| DC Ecology R||
| DC Ecology Python||
| DC Social Sciences R (Python version is not official)||
| DC Geospatial (R only)||
| DC Genomics (non-R only)||

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

From there, the project for the learner can be set up and committed.

[rstudio-cloud]: https://rstudio.cloud
[my-binder]: https://mybinder.org

