INTRODUCTION TO SOFTWARE ENGINEERING

ASSIGNMENT

OLIVER KOT 
STUDENT ID: 21000599
Class 23, room 314 218 
tuesday 12pm-2pm

Introduction
In this assignment I have made decisions to implement features based on useability, modularity and usefulness. By implementing functionalities such as unit conversion, case conversion and separation of numeric and non-numeric values, The code is able to do a variety of things whilst not using large amounts of resources. The code also contains the ability to find if numbers are valid or invalid and find numeric values in strings. These are all modular, meaning that when one feature is active the others are only used if also being used. This use of modularity allows for code to not have to rely on anything other than what is absolutely necessary.

Preliminary description and checklist
-   Code will have 5 major parts split into modules
-	Each module will contain code for one function necessary.
-	Modules will be called in a main file where users will have option to choose what they want to use.
-	Modules will be named after each function required for organisation.
o	Numbers – splits numbers and letters
o	Valid – validates numbers
o	Length converts measurements of lengths
o	Case – conversion of upper/lower case
o	Numrem – removes numbers for case transition
o	Main – main file that imports rest of code
-	Main file will print options where users can choose what they want to execute, choice will only execute that module.
-	All results will be printed.

Modularity checklist
	Code must be modular 
	Code must be cohesive with very little unnecessary code
	If a module is being used the entire module is being used.
	Coupling must be loose
	Code must be easy to read and use
•	Code follows all in checklist


Testing

Testing designs
Whilst testing the code, there were many checks that I went through to enure it would not fail for each module.

- case conversion module
    - returns to input when numeric values entered - passed
    - converts lower to uppercase - passed
    - converts upper to lowercase - passed
    - gives option to convert more after completing task - passed

- unit conversion module
    - converts meters to feet, centimeters, inches accurately - passed
    - converts feet to meters, inches, centimeters accurately - passed
    - converts inches to meters, feet, centimeters accurately - passed
    - converts centimeters to meters, feet, inches accurately - passed
    - gives option to convert more after completing task - passed
    
- removing numbers for case conversion module
    - removes numeric values when combined with non-numeric values - passed
    - after removing numeric values, gives option to convert to upper/lowercase values - passed
    - removes symbols aswell as numeric values. - passed
    - gives option to convert more after completing task - passed
    
- validating number module
    - considers numeric values combined with digits, relevent symbols etc to be valid - passed
    - returns to input if given non-numeric values - passed
    - prints error statement when given invalid numeric values - passed
    - gives option to validate more after completing task - passed
- finding numeric value module
    - finds numeric values within strings - passed
    - splits numeric and non-numeric values in given string - passed
    - prints numeric values in string - passed
    - prints non-numeric values in string - passed
    - gives option to go again after completing task - passed
- main module
    - imports all five modules - passed
    - runs menu on startup for user to decide call each module as needed - passed
    - only executes module when module is called by user - passed
    - when module is passed, only that module runs. - passed
    - returns to menu - failed

Use of White box testing
-
white box testing would be beneficial for the numeric value remover module and the numeric validation module. these modules would benefit as being able to see what leads to the output is crucial as there is mathematical equations involved. this code is necessary for the modules to run and it is necessary to be able to test that the numbers printed match input values and external sources that aim to do the same thing such as a calculator.

Test results
-
- tests were conducted regarding the testing phase above^
- case conversion module - all passed
- unit conversion module - all passed
- removing numbers for case conversion module - all passed
- validating number module - all passed
- finding numeric value module - all passed
- main module 
    - all passed except one 
    - the only failed test was the return to menu once work was completed.

the test results were more than successful with a program and modules that all work well and in sync, with no issues other than the main file not returning when the module closed.


	

Ethics and professionalism
-
The code that I have designed could be used in multiple ways in a large software project. With the main useful functions being the unit conversions. However if used unethically or unprofessionally it could be damaging to a project. due to the use of the git version control system, this code is traceable to whoever edits or changes any parts of it when it is used responsibly. If an employee or team member make malicious changes or changes that are not logged or traceable it can lead to other team members being held responsible and depending on the extent, lead to termination of employment. In order to ensure that this does not happen, all team members who have access to the project must undergo training that teaches them the importance of ethical behaviour in the workplace and the importance of commiting all changes to projects. It is also important that the team members are aware that their actions can impact their coworkers and jeopradise the entire project.

Guide to running code
- 
- first of all you will need to download the zip file containing the code
- once completing this unzip the modules and open the "main" module. this module will be what you use to access everything.
- once opening the main module you will be given 5 options
    - 1 - Convert a string to Upper or Lower Case
    - 2 - Identify if a String contains Numeric Values
    - 3 - Identify whether a given string is a valid number
    - 4 - Remove numeric values from a string for Case Conversion
    - 5 - conversion of measurements
    - 0 - exit

from this point you input numbers 1-5 depending on what you would like to do. (note, if a value is entered that is not visible. an error message will appear and send the user back to the menu)

now depending on your choice different things can happen.
- if you chose to Convert a string to Upper or Lower Case.
    -  you will be asked to "enter a string" 
    -  now enter what you want to convert. 
    -  you will now be given the option to convert to upper or lower case.
    -  select the case you want to convert to and it will be converted. 
    -  you will then be given the option to convert more, if you choose yes, you will be returned to the "enter a string" message, if you choose not to, the program will quit.

- if you chose to Identify if a String contains Numeric Values
    - you will be asked to "enter a string"
    - then depending on what you entered, you will recieve both numeric and non-numeric values split apart.
    - if values that are neither numeric or non-numeric, e.g. symbols you will recieve an error message and sent back to "enter a string"
    - once you have recieved your results you will then be given the option to convert more, if you choose yes, you will be returned to the "enter a string" message, if you choose not to, the program will quit.

- if you chose to Identify whether a given string is a valid number
    - you will be asked to "enter a string"
    - after inputting a value you will recieve a statement that will tell you if your value is valid or not. (note that if your input contains non-numeric values of any sort, the value will automatically be regarded as invalid.)
    - after recieving your results you will be given the option to convert more, if you choose yes, you will be returned to the "enter a string" message, if you choose not to, the program will quit.

- if you choose to Remove numeric values from a string for Case Conversion
    - you will be asked to "enter a string"
    - the module will print out the non-numeric values from whatever you input. 
    - after recieving your results you will be given the option to convert to upper/lowercase.
    - once deciding what to convert to, you will be given results and asked whether you would like to do it again if you choose yes, you will be returned to the "enter a string" message, if you choose not to, the program will quit.
    
- if you choose the conversion of measurements option.
    - you will be asked what your current measurement is and given the options meters, centimeters, feet and inches.
    - once selecting your current measurement, you will be asked what measurement you would like to convert it to. 
    - after choosing the desired unit to convert to, enter the distance or measurement you want to convert and the module will print out the converted distance.
    - after recieving your results you will be given the option to convert more, if you choose yes, you will be returned to the choose your current measurement, if you choose not to, the program will quit
