<div align="center">

# ReactSPH: WIP SPH solver

</div>
The Smoothed Particle Hydrodynamics (SPH) solver <strong><em>ReactSPH</em></strong> aims to introduce chemical kinetics and combustion modeling to SPH for real world engineering applications. It is developed at the Tsue Nakaya Laboratory (津江・中谷研究室) at the University of Tokyo (東京大学).

## Table of Contents

1. [**Current TODOs**](#todos)
2. [**Installation**](#installation)


## TODOs:
Official [HackMD](https://hackmd.io/@JonasErbesdobler/rkZ7Nugz1x/edit) for extensive TODO list.

- [ ] Rewrite previous Fortran code in C++

## Installation
### CMake
In our current development chain, we use three different compiler version presets. However, they all run the same `CMakeLists.txt` file.  
`g++/gcc 14`:
```bash
cmake --preset gcc14
cmake --build --preset gcc14
```
`g++/gcc 13`:
```bash
cmake --preset gcc13
cmake --build --preset gcc13
```
`clang 18`:
```bash
cmake --preset clang18
cmake --build --preset clang18
```

### Python Utilities
If you want to use any of the Python utilties, we recommend using `Python3 venv` for building your local environment.
**Using `python3-venv`**
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
pip install -e . # to install in interactive mode
```
Later, you just need to `source venv/bin/activate` to activate the environment.