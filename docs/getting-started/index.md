# Getting Started

---

## Download and Start

Download a release from the [release page](https://github.com/power-flow-analyzer/PowerFlowAnalyzer/releases)
(e.g. [PowerFlowAnalyzer-2.3.0.zip](https://github.com/power-flow-analyzer/PowerFlowAnalyzer/releases/download/2.3.0/PowerFlowAnalyzer-2.3.0.zip)) and unzip the file. A new folder `PowerFlowAnalyzer-<VERSION>` will be created. The final name is version dependant (e.g. `PowerFlowAnalyzer-2.3.0`).

Open the newly created folder and execute the start script in Matlab:
```matlab
>> pfa_start_application.m
```
The graphical user interface (GUI) will open in a new window:
<img src="img/gui_started.png" height="200" />

## Open an example project

Click the ![open_icon](../icons/folder.png) button on the toolbar. A new window will open. 

Select or enter the path to the project file `<PATH TO PFA>/examples/matpower/matpower.case` of your PFA installation. Click `OK`.

![matpower_case_loaded](img/gui_matpower_case_loaded.PNG)

Select the item `IEEE 14 Bus Test Case` in the `Overview` area on the left side. The item will be highlighted. A network summary similar to Matpower will be show:

<img src="img/case14_network_summary.PNG" height="150" />

You can change the name of a network and add a description in the `Network information` tab:

<img src="img/case14_network_information.PNG" height="150" />

By double clicking an item in the `Overview` area, the network will be shown:
![case14_opened](img/case14_opened.PNG)

The user interface offers basically three different visualisation types for network data:

* _network maps_ drawing grid topology data and heat maps
* _network browsers_ allowing to explore data in a hyperlink like style
* _data tables_ listing specific elements and their parameters

Selecting an item in a visualisation will update all other visualisations to reflect the current selection. 

## Compute power flow with Matpower

Click the ![execute_script](../icons/script_gear.png) button on the toolbar. A dialog will open and show the available scripts. Click on `2. Calculate Power Flow`.

<img src="img/gui_select_script.PNG" height="200" />

The script parameter dialog will show up. Select `AC Standard` as the power flow algorithm. Click `OK`.

<img src="img/gui_calc_powerflow.PNG" height="200" />

This particular script will perform the following actions:

* convert network data into the Matpower case format
* compute power flow using Matpower functions
* convert calculation results into network data
* update user interface

Take a look at the Matlab console to view the logging output of the PFA and Matpower functions. 

![case14_pf_results_no_selection](img/case14_pf_results_no_selection.PNG)

Click on one of the red dots in the network viewer to see which constraint was violated:

![case14_pf_results_select_gen1](img/case14_pf_results_select_gen1.PNG)


## Load other IEEE Test Cases

Switch back to the `Overview` panel and select the action `Create empty network`:

<img src="img/gui_select_action_with_selection.PNG" height="120" />

Now execute the script `1. Import Matpower Case`:

<img src="img/gui_select_action_or_script.PNG" height="120" />

The script parameter dialog will show up. Select an input Matpower case (e.g. `IEEE 30 Bus Test Case`). Click `OK`.

<img src="img/gui_load_test_case.PNG" height="150" />

Select the newly created network in the list, change its name and view it by double clicking on it's list item.

![case30_show_results](img/case30_show_results.PNG)

Grouping assets by specific models or parameters may reduce significantly the information shown in the user interface. Take a look at the bus section in the `Network Overview`:

<img src="img/case30_buses.PNG" height="120" />

Clicking on one of these items will select/highlight the items in this group:

![case30_show_results_select_area1](img/case30_show_results_select_area1.PNG)
