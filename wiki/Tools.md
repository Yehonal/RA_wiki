# Additional River Architect Tools

*Tool* scripts can be considered as beta versions of future functionalities that will be implemented in *River Architect*. Typically, *Tools" are basic commandline scripts for creative design support. Currently, routines for the hydraulic design of pool-riffle sequences or flood analysis are available, where the flood analysis applies to the U.S. Army Corps of Engineers' [`HEC-SPP`][hecspp] software. The *Tools* routines are located in `RiverArchitect/Tools/`. 

# Scripts

## Main Tool scripts

Run the following scripts with Esri's *Python* environment ([read more](Installation#raenv))

 - `make_annualpeak.py` prepares required input data for statistic flow analyses and with the U.S. Army Corps of Engineers' [`HEC-SPP`][hecspp] software.

 - `make_flowduration.py` creates flow duration curves (annual averages) for the assessment of AUA.

 - `morphologydesigner.py` creates design tables for self-sustaining pool-riffle channels (uses `cHydraulic.py` and `cPoolRiffle.py`).

 - `run_make_….bat` are a batchfiles that run `make_….py` on Windows x64.

 - `run_morphology_designer.bat` is a batchfiles that runs `morphology_designer.py` on Windows x64.
 

## Class and Function files

The code execution depends on the following folders and scripts:

 - `.templates` folder contains a template workbooks for multiple purposes.

 - `Products` folder contains results of any script in this folder.

 - `cHydraulic.py` contains a class with routines for calculating cross-section-averaged flow characteristics.

 - `cInputOutput.py` contains classes required for reading and writing data, as well as calculation progress logging.

 - `cPoolRiffle.py` provides routines for designing self-sustaining pool-riffle channels.

 - `fTools.py` is a set of functions used by other Python applications within this folder.
 

[1]: https://github.com/RiverArchitect/Welcome/wiki/Installation
[2]: https://github.com/RiverArchitect/Welcome/wiki/Signposts
[3]: https://github.com/RiverArchitect/Welcome/wiki/LifespanDesign
[4]: https://github.com/RiverArchitect/Welcome/wiki/MaxLifespan
[5]: https://github.com/RiverArchitect/Welcome/wiki/ModifyTerrain
[6]: https://github.com/RiverArchitect/Welcome/wiki/HabitatEvaluation
[7]: https://github.com/RiverArchitect/Welcome/wiki/ProjectMaker
[8]: https://github.com/RiverArchitect/Welcome/wiki/Tools
[9]: https://github.com/RiverArchitect/Welcome/wiki/FAQ
[10]: https://github.com/RiverArchitect/Welcome/wiki/Troubleshooting

[wyrick14]: https://www.sciencedirect.com/science/article/pii/S0169555X14000099
[hecspp]: https://www.hec.usace.army.mil/software/hec-ssp/