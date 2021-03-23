`pyro` is a PDE solver constructed in Python, so it most likely falls under the category of "programming tool". PDE's appear in a variety of physics fields, including waves, diffusions, transports, and quantum mechanics. `pyro` has a number of PDE solvers at its disposal, making it a tool that can assist in solving and displaying several physics problems.

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

With the proper screen resources, this should display a pulse moving diagonally through the image. This serves as a quick unit test to ensure that all the necessary packages/libraries (`numpy`, `numba`, `matplotlib`, `h5py`) are installed.

All of the main files are located in (and can be run from) the main directory.

* Repositories:
  * Main `pyro` repo: https://github.com/python-hydro/pyro2
  * Project repo: https://github.com/priesbr1/CMSE401_pyro2_project

* Documentation:
  * `pyro` documentation: https://pyro2.readthedocs.io/en/latest/intro.html
  * `pyro` main README: https://github.com/python-hydro/pyro2/blob/main/README.md

* Usage:
   * `pyro` setup/testing: https://pyro2.readthedocs.io/en/latest/installation.html
   * Running `pyro`: https://pyro2.readthedocs.io/en/latest/running.html
