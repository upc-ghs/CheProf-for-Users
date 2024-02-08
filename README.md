# CheProf-for-Users
This repository contains documentation and executables for CheProf, a platform for hydrogeochemical calculations. There are four simple (1D) codes: 
1. CheProfRW. It just reads xml files for a chemical system and local chemistries and writes them again in xml format. This can be useful when one wants to convert a case calculated by, e.g., Phreeqc, into xml files through the PhreeqcFile attribute in the chemical system and/or local chemistries. The output files contain the full chemical system and/or local chemistries with information obtained from Phreeqc. This information can be checked, adjusted and/or extended for subsequent use by other codes. The source code for developers can be find at https://github.com/upc-ghs/CheProfRW.
2. ChemMix. ChemMix calculates the chemical composition of the mixing of two end members (local chemistries) with various mixing ratios.  The source code for developers can be find at https://github.com/upc-ghs/ChemMix.
3. DSA1D. It calculates reactive transport in a one-dimensional domain discretized by finite elements using the Direct Substitution Approach (DSA). Transport includes advection, diffusion and dispersion in only the liquid phase. Liquid flow is assumed uniform in space, but it may vary in time. The source code for developers can be find at https://github.com/upc-ghs/DSA1D.
4. WMA1D. It uses the Water Mixing Approach to solve reactive transport in a simple one-dimensional domain with uniform flow of water. The source code for developers can be find at https://github.com/upc-ghs/WMA1D.

Each code has a folder with examples and with executables for both MS-Windows ((name of code)Win.exe) and Unix ((name of code)Unix). In MS-Windows the examples can be executed by double clicking on the file "Run(name of code)Win.bat" in the folder of each example.

Input for codes is done with xml input files. These files can best be viewed and edited by means of Notepad++, which is most probably already installed on your computer. If not, it can be downloaded from https://notepad-plus-plus.org/. To take advantage of the XML language, it is recommended to install the plugin "XML Tools" in Notepad++. To do so start Notepad++ and navigate to "Plugins" ->"Plugins Amin...", search "XML Tools" in the list of all available plugins. Select the checkbox. Click the "Install" button to complete the installation of XML Tools. XML Tools can be used to check the XML language, that is, to check whether the file is written in a correct XML format. To do so, click "Plugins" -> "XML Tools" -> "Check XML syntax now". XML Tools can be used also to validate the file, that is, to check whether the file is written according to the CheProf input file description explained in the documentation. To do so, click "Plugins" -> "XML Tools" -> "Check XML syntax now". It will ask to "Please select XML schema (XSD)". Then select the file "CheProf.xsd" from the main folder "CheProf_for_Users".

More information and a detailed input file description can be found in the Documentation.pdf at the main folder "CheProf-for-Users".
