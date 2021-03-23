# Pyro Project

## Abstract

`pyro` is a PDE solver constructed in Python, so it most likely falls under the category of "programming tool". PDE's appear in a variety of physics fields, including waves, diffusions, transports, and quantum mechanics. `pyro` has a number of PDE solvers at its disposal, making it a tool that can assist in solving and displaying several physics problems.

## Installation

`pyro` is a GitHub repository, primarily built and maintained by Michael Zingale. For the main `pyro2` repository, you can install it on the HPCC using

```bash
git clone https://github.com/python-hydro/pyro2 <target_directory_name>
```

For my version (forked from the main repository), you can use

```bash
git clone https://github.com/priesbr1/CMSE401_pyro2_project <target_directory_name>
```

Once in the main directory, run the command

```bash
./pyro.py advection smooth inputs.smooth
```

With the proper screen resources, this should display a pulse moving diagonally through the image. This serves as a quick unit test to ensure that all the necessary packages and libraries (`numpy`, `numba`, `matplotlib`, `h5py`) are installed.

## Example Code

All of the main files are located in (and can be run from) the main directory. When running from the command line, you need three basic inputs:

```bash
./pyro.py <solver> <problem_type> <problem_input>
```

Here, `solver` is one of the solvers that `pyro` supports. Each solver has a folder available in the main directory (e.g. `advection`, `compressible`, `diffusion`, etc.). The availability of `problem_type` and `problem_input` will depend on the solver, but the options for each can be found in the solver's `problems` subdirectory.

As an alternative, `pyro` can also be run using the `Pyro` class in a Python script. `examples.ipynb` in the `examples` directory gives a walkthrough for how this works.

## Submission Script

To run the submisson script, run `pyro_advection_smooth.sb` from the `CMSE401_deliverables` directory. This will submit the test case (see **Installation**) as a job to the HPCC. All of the output will be located in the `CMSE401_deliverables` directory.

## References

* Repositories:
  * Main `pyro` repo: https://github.com/python-hydro/pyro2
  * Project repo: https://github.com/priesbr1/CMSE401_pyro2_project

* Documentation:
  * `pyro` documentation: https://pyro2.readthedocs.io/en/latest/intro.html
  * `pyro` main README: https://github.com/python-hydro/pyro2/blob/main/README.md

* Usage:
   * `pyro` setup/testing: https://pyro2.readthedocs.io/en/latest/installation.html
   * Running `pyro`: https://pyro2.readthedocs.io/en/latest/running.html
