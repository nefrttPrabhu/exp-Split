Expense Splitter Service
Overview
The Expense Splitter Service is a single-page web application built to help small groups, like roommates or friends on a trip, to easily track shared costs and determine who owes whom. It eliminates the need for manual calculations or confusing spreadsheets by providing a clean, intuitive interface to log expenses and automatically calculate balances and settlements.



Features
Group Management: Simple interface to add members to your group one by one.


Dynamic Expense Logging: Record expenses with a description, amount, and specify who paid.


Flexible Splitting: Select exactly which members of the group should share the cost of each specific expense.


Real-Time Balance Calculation: The application automatically calculates and displays each member's running balance—showing if they are owed money or if they owe money to the group.



Optimized Settlements: Generates a clear, minimal list of payments required for everyone to settle their debts and get back to zero.


Instant UI Updates: The entire dashboard, including expenses, balances, and settlements, updates instantly without needing to refresh the page.

How to Use
Add Group Members:

In the "Add Member" panel, enter a name into the input field and click the "Add to Group" button.

Repeat this for all members you want to include.

Record an Expense:

Move to the "Add Expense" panel.

Fill in the Description, Amount, and select who Paid By from the dropdown menu.

Under Split Between, check the boxes next to the names of all the people who are sharing this particular expense.

Submit the Expense:

Click the "Record Expense" button.

Review the Summary:

The expense will immediately appear in the "Recent Expenses" list.

The "Balances" and "Settlements" panels will automatically update to reflect the new calculations.

Installation
This is a standalone front-end application with no server-side dependencies.

Download the index.html file to your local machine.

Open the index.html file directly in any modern web browser (like Chrome, Firefox, or Edge).

Code Highlights
HTML provides the application's structure.

CSS is embedded directly in the HTML file for styling, creating a clean and responsive user interface without external libraries.

Vanilla JavaScript powers all the dynamic functionality of the application. There are no external frameworks or libraries like jQuery or Bootstrap.

Key JavaScript Functions
addMember(): Adds a new person to the group, updating the UI and the underlying members array.

addExpense(): Validates and adds a new expense to the expenses array, then triggers updates across the UI.

recalculate(): The core function that is called after any change. It computes all balances from scratch and calls the display functions.

displayBalances(): Renders the summary of what each person owes or is owed.

displaySettlements(): Implements a greedy algorithm to calculate the minimum number of transactions needed to clear all debts and displays them.

Example Use Case
Imagine four roommates—Alice, Bob, Carol, and Dave—are using the app.

Alice buys $100 worth of groceries for everyone. She adds an expense, sets herself as the payer, and checks all four names under "Split Between".

Later, Bob pays a $60 utility bill that is only for him and Alice. He adds this expense, sets himself as the payer, and checks only his and Alice's names.

The app automatically calculates the final balances. For instance, Alice might be owed $15, Bob owed $5, while Carol and Dave each owe $10. The "Settlements" panel would then clearly suggest that Carol pays Alice $10 and Dave pays $5 to Alice and $5 to Bob to settle up.

Screenshots
(This is where you would place screenshots of your application in action)

<img width="1680" alt="Application showing members and expenses" src="https://via.placeholder.com/1680x900.png?text=App+Screenshot+1">
<img width="1680" alt="Application showing balances and settlement details" src="https://via.placeholder.com/1680x900.png?text=App+Screenshot+2">

Technologies Used
HTML5

CSS3

Vanilla JavaScript

License
This project is licensed under the MIT License. Feel free to use and modify it as per your requirements.
