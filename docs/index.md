# Power Flow Analyzer

Toolbox for power system analysis

---

PowerFlowAnalyzer (PFA) is a toolbox for the analysis of power systems, written in Java and Matlab. Its main focus is the modelling and visualisation of network data for transmission and distribution grids. 
It interfaces Matlab and Matpower for computations and integrates various data sources (CSV, Excel, UCTE DEF, QGIS). PFA has its roots at the [Technische Universit&auml;t Berlin](https://www.tu-berlin.de) and was used in several research projects and student theses relating grid planning and operation topics. 

PFA is free software: you can use it, modify it and redistribute it under the terms of the [Apache License, Version 2.0](license/license.md).

Source code, documentation and build files are available at [github.com/power-flow-analyzer](https://github.com/power-flow-analyzer).

---

## Features

### Core Features
* explorative graphical analysis of transmission and distribution grid data
* definition of custom workflows using configurable Matlab scripts
* Matpower integration for computing (optimal) power flows
* management of projects, networks, scripts and parameters
* graphical user interface (GUI) for management and analysis tasks

### Visualisations
* visualise grid topology and regions using geographic maps
* explore grid characteristics using the network browser
* use heat maps to analyze trends and patterns in large systems
* draw direction of (active) power flow on all lines
* define custom error levels and their visualisation for all grid assets
* aggregate and filter network data at multiple levels (e.g. operator, region, substation or voltage level)

### Interfaces
* Matlab: generic interface for defining parameters and executing functions graphically
* Matpower: compute (optimal) power flow, PTDFs, LODFs, ...
* Excel: optimised loading routines for easy and fast data access
* UCTE DEF: import grid data suitable for grid operators

### Runtime Environment
* no installation required: download, unzip, start in Matlab
* workflows may be intiated from GUI and/or in batch processing
* platform independant due to its nature, although only Windows is tested

### License
* open source license (Apache Version 2.0), suitable for education, research and enterprises
* the full source code, documentation and build files are available for download from Github

---

## Installation

No installation is required, just download, unzip and start in Matlab.

### Download
Download a release from the [release page](https://github.com/power-flow-analyzer/PowerFlowAnalyzer/releases)
(e.g. [PowerFlowAnalyzer-2.3.0.zip](https://github.com/power-flow-analyzer/PowerFlowAnalyzer/releases/download/2.3.0/PowerFlowAnalyzer-2.3.0.zip)).

### Unzip

Unzip the zip file. A new folder `PowerFlowAnalyzer-<VERSION>` will be created. The final name is version dependant (e.g. `PowerFlowAnalyzer-2.3.0`).

### Start in Matlab

Run `pfa_start_application.m` in Matlab.

---

## License

PowerFlowAnalyzer is released under the Apache License, Version 2.0 (see [LICENSE file](license/license.md)).
You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.

This software includes [MATPOWER](http://www.pserc.cornell.edu/matpower) 
[(Github)](https://github.com/MATPOWER/matpower "MATPOWER on Github"), 
[MigLayout](http://miglayout.com) [(Github)](https://github.com/mikaelgrev/miglayout "MigLayout on Github") and [Fatcow Hosting Icons](http://www.fatcow.com) 
[(Github)](https://github.com/ioBroker/ioBroker.icons-fatcow-hosting "Fatcow Hosting Icons on Github").
See [NOTICE file](license/notice.md) for more information. 
