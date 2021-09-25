FROM jupyter/minimal-notebook:notebook-6.4.4

ARG NB_USER=jovyan
ARG NB_UID=1000

COPY . /home/${NB_USER}

USER root
SHELL ["/bin/bash", "-c"]
RUN apt-get update && apt-get install --no-upgrade --no-install-recommends -y libgl1-mesa-dev && \
    apt-get clean && \
    apt-get autoremove -y && \
    rm -rf /var/lib/apt/lists/* && \
    mamba env update -n base -f /home/${NB_USER}/binder/environment.yml && \
    jupyter lab build && jupyter lab clean

RUN chown -R ${NB_UID} /home/${NB_USER}
USER ${NB_UID}
WORKDIR /home/${NB_USER}/notebooks
