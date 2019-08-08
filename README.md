# RapidMax

This is the RapidLib C++ machine learning library wrapped into a Max/MSP object, for use with Windows.
(http://gitlab.doc.gold.ac.uk/rapid-mix/RapidLib)

Access to the MacOS RapidMax repo can be found here:
https://github.com/samparkewolfe/RapidMax

## Compiling

Visual Studio solution and project files are located inside /rapidmax/.

The solution file contains the relative file path info needed to compile and build the Max x64 External object. On building, a bin folder will be created and the rapidmax object will be placed inside.

Ensure you have pulled the submodule RapidLib. 

## De-bugging

If met with the compilation error C2039 referring to the [searchWindow.cpp] file: include the algorithm header to this file, clean the solution, and rebuild. 
 
## Using in a Max/MSP Project

### Allow the rapidmax helpfile to be accessed from within a Max project:

* Inside your packages folder (/Users/MyDocuments/Max8/Packages), designate a new folder for your new rapidmax object, and name it something like 'rapidmax'
* Create a subfolder 'externals' and place the rapidmax x64 file inside here
* Also place the folder named 'help' from this repo alongside the 'externals' folder

Now alt-clicking on the rapidmax object (in Max) should present you with the help file.