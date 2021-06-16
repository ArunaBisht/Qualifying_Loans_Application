# Project Title - Loan Qualifier Application

Snapshot.PNG

The objective of this project is to find out which users qualified for the loan given the matrix of- credit score, max DTI, max LTV, max loan amount. Second is- non technical users will automatically save their qualifying loans into the csv file. 

Inspiration for this project - this project automize the manual work of who or who's not qualified and automatically save it in csv form the users in the presentable form.

---

## Technologies

Language used is Python. 

Libraries used are - sys, fire, questionary, path. We have used module concept in this code and under each module there are different functions, which are pulled into main file - app.py. Following are the modules - (1) credit_score.py (2) debt_to_income.py (3) loan_to_value.py (4) max_loan_size.py (5) calculators.py (6) fileio.py (7) test_qualifier.py. 

Operating system used is Windows.

Version of the python is - Python 3.8.5

Dependencies - 
testpath==0.4.4
questionary==1.9.0
pytest==0.0.0
pathlib2==2.3.5
pathtools==0.1.2
packaging==20.4
pandas @ file:///C:/ci/pandas_1602083338010/work
pandas-datareader==0.9.0
fire==0.3.1

## Installation Guide

We have to install libraries (1) 'questionary (version==1.9.0)'- this library is used to ask questions as seen below and which ever has function (ask())

    credit_score = questionary.text("What's your credit score?").ask()
    debt = questionary.text("What's your current amount of monthly debt?").ask()
    income = questionary.text("What's your total monthly income?").ask()
    loan_amount = questionary.text("What's your desired loan amount?").ask()
    home_value = questionary.text("What's your home value?").ask()
    csvpath = questionary.text("Enter a file path to a rate-sheet (.csv):").ask()
    response = questionary.confirm("Would you like to save your loan data as a .csv file? ").ask()

    (2) Library 'SYS' (version==0.5.1)- this mostly provides information about the constraint, functions and methods of interpreter

    (3) Library 'Fire' (version==0.3.1) - this is use to turn the python component into command line interface

    (4) Library path (version==2.3.5)

Here is the snapshot of the module structure and functions under each module.

![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/Modules_snapshot.PNG)

---

## Examples

Following snapshot shows how the code is structured and what functions fall under each module. 
(A)Module Utility - this means the pipeline for extrating the data and hence these function (i) calculating.py (ii) fileio.py is used
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/calculators.PNG)
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/fileio.PNG)

(B) Module Filter - this modules has functions which filters the data based upon the data entered by the 

![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/max_loan_size.PNG)
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/loan_value.PNG)
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/debt_income.PNG)      
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/credit_Score.PNG)

(C) Module Test - this module is used for the unit test
(D) Module Data - this module has the data in the excel file
(E) APP.PY - this is the main file which calls all the modules and there corresponding functions.

![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/Snapshot.PNG)

This shows that code is running fine and all the values enter by the user is saved to the csv file.

![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/Snapshot.PNG)

## Usage

This shows that code is running fine and all the values enter by the user is saved to the csv file.
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/qualifying_loans.PNG)
![Image](https://github.com/ArunaBisht/Projects/blob/main/Challenge_2_folder/Snapshot.PNG)

---

## Contributors

Answer. I did this project by myself and doubts were clarified by instructor.
Email - aarunabisht@gmail.com

---


## License

When you share a project on a repository, especially a public one, it's important to choose the right license to specify others what they can and can not do with your source code and files. Use this section to include the licence you want to use.

There is no license
