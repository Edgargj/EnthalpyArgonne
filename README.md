# EnthalpyArgonne

EnthalpyArgonne is a program that calculates molecular enthalpies of formation at 298.15 K, using the output of the Gaussian09 package. To compute the enthalpies, the program uses internally atomization reactions. In addition, experimental data of gaseous atoms at 0 K are taken from Argonne Thermochemical Tables (https://atct.anl.gov). Thermal corrections for elements in their standard state at 298.15 K are taken from NIST-JANAF Thermochemical Tables J. Physics Chem. Data Monograph 9, 1998, 1-1951. The program supports the following composite methods: G3, G3MP2, G4, CBS-APNO and CBS-QB3. 

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

