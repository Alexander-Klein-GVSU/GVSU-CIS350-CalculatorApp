# Overview
This document lists the functional and non functional requirements of our project.
The functional requirements list what the program needs to do when the user interacts with it.
The non functional requirements list how the program should run when interacted with.

# Software Requirements
In each section of this portion, each header represents one feature of the app. It then shows a table of the specifications and tests of each feature.

## Functional Requirements
### Calculator App
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR1 | User shall be able to get to every part of the app through basic navigation. | N/A |
### Step-by-Step
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR2 | Step-by-step shall allow users to input any number they want into input boxes. | TC6 |
| FR3 | Step-by-step shall output answers in a cohesive way so the user can understand how to do the calculation themselves. | N/A |
| FR4 | User shall be able to go back to other functions of the app from the step-by-step portion. | N/A |
### Basic Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR5 | Basic calculator shall handle basic addition, subtraction, multiplication, and division manipulation of variable input by the user | TC7, TC8, TC9, TC10|
| FR6 | User shall be able to use the previous output as starting number for next calculation. | TC3 |
### Menu
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR7 | User shall be able to press buttons on the menu screen to access different parts of the code. | TC13 |
### Graphing Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR8 | The graphing calculator shall solve and graph functions inputted by user. | TC14 |
| FR9 | The graphing calculator shall display solutions to systems of equations when the user enters multiple functions. | N/A |
| FR10 | The graphing calculator shall zoom in and out if the user chooses. | N/A |
### Calculus
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR11 | User shall input a function into a text-box. | TC1 |
| FR12 | User shall select a calculus option (ex: 1st derivative, nth derivative). | TC5 |
| FR13 | User shall be able to click on calculus option in menu to go to calculus calculator. | TC11 |
| FR14 | User shall be able to click the simplify button to simplify small equations. | N/A |
### Hypergeometric Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| FR15 | User shall be able to calculate the probability of getting a card within a certain number of turns. | TC4 |

## Non-Functional Requirements
### Calculator App
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR1 | App shall have fast and seamless transitions from one part of the app to another. | TC15, TC16 |
| NFR2 | App shall be allowed to run on many different android devices. | TC17 |
### Step-by-Step
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR3 | User shall not be able to enter non-numbers into the input boxes for step-by-step. | TC18 |
### Basic Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR4 | Program shall be able to detect if an input is valid or invalid. | N/A |
| NFR5 | Basic calculator shall have a shared display screen for user inputs and outputs. | TC19 |
### Menu
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR6 | Menu shall seamlessly move to and from different section of the program. | N/A |
### Calculus
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR7 | An output display shall update with a solution when a valid function is entered along with a calculus option being selected. | TC2 |
| NFR8 | The app once in the calculus portion shall be able to go back to the main menu. | TC12 |
### Graphing Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR9 | The graphing calculator shall graph separate lines in different colors. | N/A |
| NFR10 | The graphing calculator shall look clean. | TC20 |
### Hypergeometric Calculator
| ID | Requirement | Test Cases |
| :-------------: | :----------: | :----------: |
| NFR11 | The hypergeometric calculator shall be accruate and polished. | N/A |
| NFR12 | The hypergeometric calculator shall be easy to use. | N/A |

# Test Specification
This portion of the document aims to show the number of tests that have been done throughout the project that test the truthfulness and accuracy of our above requirements.
## Unit tests
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC1 | User shall input a function into a text-box. | Navigate to calculus calculator. enter a value in text box and press any derivative button | x^2 | 2x | 2x | pass | FR11 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC2 | Take an input from text box and ouput the correct output based on the option that is selected | Navigate to calculus calculator. enter a value in text box and press any simplify button | 2+2 | 4 | 4 | pass | NFR7 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC3 | Basic calculator can take input from previous calculation and use it as input for next calculation. | Navigate to basic calculator and enter 2+2 and enter. | 2+2 = 4, 4+2| 6 | 6.0| pass | FR6 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC4 | Calculate the odds of drawing a card | Must be in hypergeometric portion, then enter # cards, # of copies, and # of draws. | 52, 4, 1 | 7.69 | 7.69 | pass | FR15 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC5 | Take derivative of equation | must be on calculus portion. input an equation into text box then select derivative button | 4x^3+2x^2 | 12x^2+4x | 12x^2+4x | pass | FR12|
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC6 | Any number can be put into input boxes. | In the menu, navigate to the sample mean of the step-by-step formulas. Enter any number(s) into the text box and press "Add". | 2, 5, 2.2235, -2.964 | 1.564875 | 1.5648749999999999 | Pass | FR2 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC7 | Calculator can handle addition. | Navigate to calculator and add 2 values together. | 8 + 7 | 15 | 15.0 | Pass | FR5 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC8 | Calculator can handle subtraction. | Navigate to calculator and subtract 2 values from each other. | 45 - 37 | 8 | 8.0 | Pass | FR5 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC9 | Calculator can handle multiplication. | Navigate to calculator and multiply 2 values together. | 16 x 25 | 400 | 400.0 | Pass | FR5 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC10 | Calculator can handle division. | Navigate to calculator and divide 2 values from each other. | 4 / 20 | 0.2 | 0.2 | Pass | FR5 |
    
    
## Integration tests
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC11 | Enter calculus screen | click on calculus calculator in main menu | Press calculus calculator  | calculus layout | calculus layout | pass | FR13 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC12 | return to main menu from calculus portion | Must be in calculus portion, then click back button | click back button | main menu layout | main menu layout | pass | NFR8 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC13 | can enter any portion of code from main menu | click on any button in main menu | click on step-by-step button | step=bystep menu | step by step menu | pass | FR7 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC14 | graph an equation | Enter graphing calculator. Enter a linear function in text box and and click graph  | 2x+1 | graph representation of 2x+1 | graph representation of 2x+1 | pass | FR8 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC15 | Enter quadratic menu from main menu | In main menu select step by step. Then click quadratic formula | click step by step then quadratic formula | quadratic layout | quadratic layout | pass | NFR1 |
    
    
## System tests
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC16 | App has fast and seamless transitions. | Enter any portion of the app and be able to get out without issue. | Press a navigation button in the menu and find a way back. | Seamless navigation. | Seamless navigation. | Pass | NFR1 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC17 | App should be able to run on many different android devices. | Attempt to run the app on different devices. | Ran on physical S8+. Run on emulators of other models. | App runs smoothly on all. | App runs smoothly on all. | Pass | NFR2 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC18 | User can't enter non numbers in SBS. | Go into any SBS feature and enter an invalid number. | ., -. | App outputs message. | App outputs message. | Pass | NFR3 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC19 | Input and output of calculator should be the same window. | Open calculator, enter an equation, hit equal sign. | 6+7= | 13 appears in same window. | 13.0 appears in same window. | Pass | NFR5 |
    
| ID | Description | Steps | Input Values | Expected Output | Actual Output | Pass/Fail | Requirement Link |
| :-------------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: | :----------: |
| TC20 | The graphing calculator should easily graph basic funtions. | Enter graphing calculator, input 1x+2, press "+", press "Graph". | 1x+2 | A graph of y = x + 2. | A graph of y = x + 2. | Pass | NFR10 |
    
    
# Software Artifacts
This portion provides links to our artifacts that we have created throughout the semester.
* [Calculus Use Case](https://github.com/Alexander-Klein-GVSU/GVSU-CIS350-CalculatorApp/blob/master/notprogram/artifacts/use_case_diagrams/CalculusUseCase.pdf)
* [Graphing Calculator Use Case](https://github.com/Alexander-Klein-GVSU/GVSU-CIS350-CalculatorApp/blob/master/notprogram/artifacts/use_case_diagrams/GraphingCalculatorUseCase.pdf)
* [Use Case Description for Graphing Calculator](https://github.com/Alexander-Klein-GVSU/GVSU-CIS350-CalculatorApp/blob/master/notprogram/artifacts/use_case_diagrams/UseCaseDescriptionGraphingCalc.md)
* [Step By Step Use Case](https://github.com/Alexander-Klein-GVSU/GVSU-CIS350-CalculatorApp/blob/master/notprogram/artifacts/use_case_diagrams/stepbystepusecase.JPG)
