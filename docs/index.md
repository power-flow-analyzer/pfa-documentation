# PowerFlowAnalyzer

---

PowerFlowAnalyzer (PFA) is a software tool for visualising and analysing different network topologies along with their data. It was developed at the Technical University Berlin with the main purpose to support actual and future research on small and large scale electrical networks (e.g. transmission and distribution networks in Germany). 

PFA allows to create powerful network diagrams with true geographic coordinates containing error flags, line flows, additional markers and border outlines. Further contour diagrams can be created to visualise trends and patterns in large scale power systems. Its user interface allows to aggregate network elements at multiple levels, such as the operator, region, substation or voltage level.
Networks and the elements they contain are defined by abstract parameters which are specified in an hierarchical database, allowing to use different sets of parameters for each network. A built-in database for standard Matpower networks is included. 

It interfaces to Matlab and allows to define and execute custom scripts with individual script parameters for e.g. the import of networks from Excel files and the calculation of power flows. 

## Features

### Core Features
* explorative graphical analysis of transmission and distribution grid data
* definition of custom workflows using predefined Matlab scripts
* Matpower integration for computing (optimal) power flows
* management of projects, networks, scripts and parameters
* graphical user interface (GUI) for management and analysis tasks

### Visualisations
* visualise grid topology and regions using geographic maps
* explore grid characteristics using the network browser
* use heat maps to analyze trends and patterns in large systems
* draw direction of (active) power flow on all lines
* define custom error levels for all grid assets
* aggregate and filter network data at multiple levels

### Interfaces
* Matlab: execute functions and define parameters graphically; generic interface for all proprietary data formats
* Matpower: compute (optimal) power flow, PTDFs, LODFs, ...
* Excel: optimised loading routines for easy and fast accesss
* UCTE DEF: import grid data suitable for grid operators

### Runtime Environment
* no installation required: download, unzip, start in Matlab
* workflows may be intiated from GUI and/or in batch processing
* platform independant due to its nature, although only Windows is tested

### License
* open source license (Apache Version 2.0), suitable both for research and enterprises
* the full source code and build files are available for download from Github
