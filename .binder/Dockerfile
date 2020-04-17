FROM rocker/binder:3.6.0
LABEL maintainer='Zhian N. Kamvar'
USER root
COPY . ${HOME}
COPY ./data ${HOME}/data
RUN chown -R ${NB_USER} ${HOME}
USER ${NB_USER}


RUN R -e "options(repos = list(CRAN = paste0('http://mran.revolutionanalytics.com/snapshot/', substring(readLines('.binder/runtime.txt'), 3, 12)))); devtools::install_deps('.binder/')"


RUN wget -O data/full.zip https://ndownloader.figshare.com/articles/2009586/versions/10 \
  && unzip data/full.zip -d data \
  && rm data/full.zip \
  && unzip data/NEON-DS-Site-Layout-Files.zip -d data \
  && rm data/NEON-DS-Site-Layout-Files.zip \
  && unzip data/NEON-DS-Met-Time-Series.zip -d data \
  && rm data/NEON-DS-Met-Time-Series.zip \
  && unzip data/NEON-DS-Airborne-Remote-Sensing.zip -d data \
  && rm data/NEON-DS-Airborne-Remote-Sensing.zip \
  && unzip data/NEON-DS-Landsat-NDVI.zip -d data \
  && rm data/NEON-DS-Landsat-NDVI.zip 

RUN exit 0
