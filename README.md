# Growing Neural Cellular Automata in JAX

Differentiable Model of Morphogenesis from [Growing Neural Cellular Automata](https://distill.pub/2020/growing-ca/) article written in JAX, Flax.

<p align="center">
<img width="800" alt="teaser" src="https://github.com/maxencefaldor/growing-ca/assets/49123210/51457e98-48bd-49a6-b792-7062b2a80ee7">
</p>

- ``Growing_Neural_Cellular_Automata.ipynb``, the original notebook
- ``Growing_Neural_Cellular_Automata_jax.ipynb``, the original notebook translated in JAX

## Installation

To run this code, you need to clone the repository and install the required libraries with:
```bash
git clone https://github.com/adaptive-intelligent-robotics/DCG-MAP-Elites
pip install -r requirements.txt
```

However, we recommend using a containerized environment such as Docker, Apptainer or Singularity. Further details are provided in the last section.

## Apptainer

To build a container using Apptainer (or Singularity) make sure you are in the root of the repository and then run:

```bash
apptainer build --fakeroot --force apptainer/container.sif apptainer/container.def
```

You can execute the container with:

```bash
apptainer -d run --app [APP NAME] --cleanenv --containall --no-home --nv container.sif
```
