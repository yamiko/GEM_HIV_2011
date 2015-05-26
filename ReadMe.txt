OVERVIEW
--------

This folder contains the GEM Cutter III version of the GEM Cutter XML authoring tool. It is designed to build GEM III instance documents. 

The file GemCutter.jar is executable and can be executed by double clicking the file 
or by running from the command line as 'java =jar GemCutter.jar"


PREREQUISITES
-------------

Java 1.6+ must be installed to run this application.
The user must have write access to the folder this application folder is located in. 


CHANGES AND FEATURES
--------------------

GEM II project folders can be converted to GEM III project folders by accessing the 
Project menu and selecting GEM II => GEM III item. The original folder can be located anywhere
in the file system. The converted folder will be copied to the GEM Cutter project folder and an
extension of "_conv" added to the name.

GEM III elements have been added to the XML tree displayed in GEM Cutter.

Code sets can be added to those elements with a Code subelement.

The logic editor was redesigned to add Drog N Drop functionality and greater flexibilty in modifying
decision logic.

Projects are loaded into GEM Cutter by selecting the project folder itself, NOT a .zip file inside the project folder.  

Project folders must be located in the same directory as the GemCutter.jar file.

Report views have been modified to include most new GEM III elements and codes and code sets.

DEVELOPER
---------

Current reports can be modified by adding a folder with the name "xsl" in the same folder as the GemCutter.jar file and placing xsl transforms in 
in this folder with the following names that correspond to the existing reports.

Report                   Transform File Name
------                   ------------------- 
Recommendations          rec_cond_imp.xsl
Actions                  action.xsl
Decision Variables       dvs.xsl
GEM-COGS                 gem-cogs.xsl
Extractor - Detailed     extractor.xsl
Extractor - Rules        rules.xsl   

The xsl files can be obtained by extracting them from the jar file. To do this, place the GEMCutter.jar file in a new folder and from the command line in this folder type

jar -xvf GEMCutter.jar

This will extract all the files and folders contained in the jar file. Use the xsl folder as the basis for making the modifications described above.

--------------------

Contact George Michel with any questions, comments, or issues:

george.michel@yale.edu

9/14/12