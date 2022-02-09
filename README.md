# EnthalpyArgonne

EnthalpyArgonne is a program that calculates the enthalpies of formation (by the Gaussian09 G3, G3MP2, G4, CBS-APNO, CBS-QB3 method) of gaseous atoms at 0 K and thermal corrections for elements in their standard state at 298.16 K from: Argonne Thermochemical Tables. 

# Git instructions

You can obtain the source code of EnthalpyArgonne as follows.
In your bash terminal type:

~~~~~~~~~~
$cd /local/path/to/EnthalpyArgonne
$git clone https://github.com/Edgargj/EnthalpyArgonne.git
~~~~~~~~~~

After this, git will transfer the source files to ```/local/path/to/EnthalpyArgonne```

## Auxiliary programs/dependencies
The following dependencies are needed:

~~~~~~~~~~
g++ std=c++11 make
~~~~~~~~~~

## Installation
For installing the program, type:

~~~~~~~~~~
$cd /local/path/to/EnthalpyArgonne
$make
~~~~~~~~~~

# Testing the suite

How to test the program (or how it should be):

~~~~~~~~~~
$./computeEnthalpyArgonne.x 4NBALa.txt

===================================================================================================
                      New calculation of molecular enthalpies of formation                         
                                                                                                   
              Enthalpies of formation of gaseous atoms at 0 K and thermal corrections              
                       for elements in their standard state at 298.15 K from:                      
                                                                                                   
                                  ARGONNE Thermochemical Tables                                    
                               Warning: sulfur is taken from NIST                                  
===================================================================================================
                                                                                                   
                                                                                                   
                                                                                                   
Heats of formation: 
0K          -36.64 kJ mol-1
0K          -8.75 kcal mol-1
                                                                                                   
Using Nicolaides method: 
298K        -59.15 kJ mol-1
298K        -14.13 kcal mol-1
                                                                                                   
Using G4: 
298K        -56.66 kJ mol-1
298K        -13.53 kcal mol-1
                                                                                                   
===================================================================================================
~~~~~~~~~~

