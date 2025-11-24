# CSE-PROJECT-VITYARTHI-MONTHLY-BUDGET-PLANNER
Monthly Budget Planner: Simple Tkinter GUI app for Python users to track monthly finances. Enter income &amp; savings %, add unlimited named expenses dynamically, get instant summary with savings, total spend &amp; balance in ₹. Sleek dark theme, input validation, zero dependencies. Perfect for beginners
Monthly Budget Planner

Overview
The Monthly Budget Planner is a desktop application built with Python's Tkinter library that helps users manage their monthly finances effectively. This intuitive GUI-based tool allows users to track their income, set savings goals, manage expenses, and view a comprehensive budget summary—all in one place.
The application provides a simple and visual way to plan your monthly budget by calculating savings based on a percentage of income and tracking multiple expense categories to determine your final balance.

Features
 Income Management: Enter your monthly income in Indian Rupees (₹)
 Savings Calculator: Set a savings percentage and automatically calculate savings amount
 Expense Tracking: Add multiple expenses with custom names and amounts
 Dynamic Expense List: Build a list of expenses during the session
 Budget Summary: View a detailed breakdown of:
•	Total income
•	Savings amount and percentage
•	Balance after savings
•	Individual expenses listed
•	Total expenses
•	Final remaining balance
 Input Validation: Built-in error handling for invalid entries
 User-Friendly Interface: Clean, dark-themed GUI with yellow accents


Technologies/Tools Used
•	Programming Language: Python 3.x
•	GUI Framework: Tkinter (built-in Python library)
•	Additional Modules:
•	tkinter.messagebox for user notifications and alerts
•	IDE/Editor: Any Python-compatible IDE (VS Code, PyCharm, IDLE, etc.)

Steps to Install & Run the Project
Prerequisites
•	Python 3.6 or higher installed on your system
•	Tkinter (usually comes pre-installed with Python)
Installation Steps
1.	Verify Python Installation
bash
python --version
or
bash
python3 --version
2.	Check Tkinter Availability
bash
python -m tkinter
This should open a small test window if Tkinter is installed correctly.
3.	Download the Project
•	Save the provided code in a file named budget_planner.py
4.	Navigate to Project Directory
bash
cd path/to/your/project
5.	Run the Application
bash
python budget_planner.py
or
bash
python3 budget_planner.py
The application window should open immediately.

Instructions for Testing
Test Case 1: Basic Budget Calculation
Steps:
1.	Enter Monthly Income: 50000
2.	Enter Saving Percentage: 20
3.	Click "Add" to add expenses:
•	Expense 1: Name = Rent, Amount = 15000
•	Expense 2: Name = Groceries, Amount = 5000
•	Expense 3: Name = Transportation, Amount = 3000
4.	Click "View Summary"
Expected Result:
------ Budget Summary ------
Income: ₹50000.00
Saving (20.0%): ₹10000.00
Balance After Savings: ₹40000.00

Expenses:
Rent: ₹15000.00
Groceries: ₹5000.00
Transportation: ₹3000.00

Total Expenses: ₹23000.00
Final Balance: ₹17000.00

Test Case 2: Input Validation - Empty Fields
Steps:
1.	Leave Monthly Income or Saving Percentage empty
2.	Click "View Summary"
Expected Result:
•	Error message: "Please enter valid numbers for income and saving %."
Steps:
1.	Try adding an expense with empty Name or Amount
2.	Click "Add"
Expected Result:
•	Warning message: "Please enter both name and amount."

Test Case 3: Invalid Data Entry
Steps:
1.	Enter Monthly Income: abc (non-numeric)
2.	Enter Saving Percentage: 20
3.	Click "View Summary"
Expected Result:
•	Error message: "Please enter valid numbers for income and saving %."
Steps:
1.	Enter expense Amount: xyz (non-numeric)
2.	Click "Add"
Expected Result:
•	Error message: "Enter a valid amount."

Test Case 4: High Expenses (Negative Balance)
Steps:
1.	Enter Monthly Income: 30000
2.	Enter Saving Percentage: 10
3.	Add expenses totaling more than ₹27000:
•	Rent: 20000
•	Groceries: 10000
4.	Click "View Summary"
Expected Result:
•	Summary displays with negative Final Balance, indicating overspending
•	Example: Final Balance: ₹-3000.00

Test Case 5: Zero Savings
Steps:
1.	Enter Monthly Income: 40000
2.	Enter Saving Percentage: 0
3.	Add expenses: Rent = 15000, Food = 8000
4.	Click "View Summary"
Expected Result:
------ Budget Summary ------
Income: ₹40000.00
Saving (0.0%): ₹0.00
Balance After Savings: ₹40000.00


Expenses:
Rent: ₹15000.00
Food: ₹8000.00

Total Expenses: ₹23000.00
Final Balance: ₹17000.00

Test Case 6: Decimal Values
Steps:
1.	Enter Monthly Income: 52500.50
2.	Enter Saving Percentage: 15.5
3.	Add expenses with decimals: Utilities = 2500.75
4.	Click "View Summary"
Expected Result:
•	All calculations handle decimal values correctly
•	Values displayed to 2 decimal places

Troubleshooting
Issue: "No module named 'tkinter'"
Solution:
•	Ubuntu/Debian: sudo apt-get install python3-tk
•	Fedora: sudo dnf install python3-tkinter
•	macOS: Reinstall Python from python.org
Issue: Application window doesn't open
Solution:
•	Ensure you're running the script with Python 3
•	Check if any firewall is blocking the application
•	Try running from command line to see error messages

Future Enhancements
•	 Add graphical charts for expense visualization
•	 Save and load budget data to/from files
•	Multi-month budget tracking
•	 Delete/edit individual expenses
•	 Export budget summary as PDF or email
•	 Theme customization options

License
This project is open-source and available for educational purposes.

Author
Created as a Python GUI project for budget management learning.

Happy Budgeting! 

