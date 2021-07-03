# Demo notebooks for [vmango-lab](https://github.com/jvail/vmango-lab)

View on nbviewer, run and inspect interactively on binder or run it locally after setting up the conda environment.


## Run on binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jvail/vmango-lab-demo/main)


## View on nbviewer

### Modularity [@nbviewer](https://nbviewer.jupyter.org/github/jvail/vmango-lab-demo/blob/main/notebooks/1-modularity.ipynb)

Visualizing a model's processes and their dependencies.

![Modularity](images/1-modularity.png)

### Mango Cycles [@nbviewer](https://nbviewer.jupyter.org/github/jvail/vmango-lab-demo/blob/main/notebooks/2-mango_cycles.ipynb)

A simulation and visualization of a mango tree through two vegetative cycles.

![Mango Cycles](images/2-mango_cycles.png)

### A Mango Orchard [@nbviewer](https://nbviewer.jupyter.org/github/jvail/vmango-lab-demo/blob/main/notebooks/3-orchard_parallelization.ipynb)

Simulation of a mango orchard with multi-model parallelization.

![Orchard](images/3-orchard_parallelization.png)

### A Use Case [@nbviewer](https://nbviewer.jupyter.org/github/jvail/vmango-lab-demo/blob/main/notebooks/4-use_case_measure_and_simulate.ipynb)

A use case from measurements in the field, data preparation to simulation.

![Use Case](images/4-use_case_measure_and_simulate.png)


## Setup a conda environment and run locally

Requires a [minicoda](https://docs.conda.io/en/latest/miniconda.html) installation.

```bash
git clone https://github.com/jvail/vmango-lab-demo.git
```

```bash
cd vmango-lab-demo
conda env create -f environment.yml
```

```bash
conda activate vmango-lab-demo
jupyter notebook
```
