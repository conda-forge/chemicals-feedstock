About chemicals-feedstock
=========================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/chemicals-feedstock/blob/main/LICENSE.txt)

Home: https://github.com/CalebBell/chemicals

Package license: MIT

Summary: Chemical database of Chemical Engineering Design Library (ChEDL)

Development: https://github.com/CalebBell/chemicals

Documentation: https://chemicals.readthedocs.io/

The chemicals library features an extensive compilation of pure component chemical data that can serve engineers, scientists, technicians, and anyone working with chemicals. The chemicals library facilitates the retrieval and calculation of:

Chemical constants including formula, molecular weight, normal boiling and melting points, triple point, heat of formation, absolute entropy of formation, heat of fusion, similarity variable, dipole moment, accentric factor, etc.
Assorted information of safety and toxicity of chemicals.
Methods (and their respective coefficients) for the calculation of temperature and pressure dependent chemical properties including vapor pressure, heat capacity, molar volume, thermal conductivity, surface tension, dynamic viscosity, heat of vaporization, relative permitivity, etc.
Methods to solve thermodynamic phase equilibrium, including flash routines, vapor-liquid equilibrium constant correlations, and both numerical and analytical solutions for the Rashford Rice and Li-Johns-Ahmadi equations. Rashford Rice solutions for systems of 3 or more phases are also available.

Data for over 20,000 chemicals are made available as local databanks in this library. All databanks are loaded on-demand, saving loading time and RAM. For example, if only data on the normal boiling point is required, the chemicals library will only load normal boiling point datasets. This on-demand loading feature makes the chemicals library an attractive dependence for software modeling chemical processes. In fact, The Biorefinery Simulation and Techno-Economic Analysis Modules (BioSTEAM) is reliant on the chemicals library for the simulation of unit operations.

The chemicals library also supports integration with Numba, a powerful accelerator that works well with NumPy; Pint Quantity objects to keep track of units of measure; and NumPy vectorized functions.

If you need to know something about a chemical, give chemicals a try.


Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=10992&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/chemicals-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-chemicals-green.svg)](https://anaconda.org/conda-forge/chemicals) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/chemicals.svg)](https://anaconda.org/conda-forge/chemicals) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/chemicals.svg)](https://anaconda.org/conda-forge/chemicals) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/chemicals.svg)](https://anaconda.org/conda-forge/chemicals) |

Installing chemicals
====================

Installing `chemicals` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `chemicals` can be installed with `conda`:

```
conda install chemicals
```

or with `mamba`:

```
mamba install chemicals
```

It is possible to list all of the versions of `chemicals` available on your platform with `conda`:

```
conda search chemicals --channel conda-forge
```

or with `mamba`:

```
mamba search chemicals --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search chemicals --channel conda-forge

# List packages depending on `chemicals`:
mamba repoquery whoneeds chemicals --channel conda-forge

# List dependencies of `chemicals`:
mamba repoquery depends chemicals --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance,
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information, please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating chemicals-feedstock
============================

If you would like to improve the chemicals recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/chemicals-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks, and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@CalebBell](https://github.com/CalebBell/)
* [@volpatto](https://github.com/volpatto/)
* [@yoelcortes](https://github.com/yoelcortes/)

