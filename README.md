Of course. Here is a README file formatted in Markdown, ready for you to upload to your GitHub repository for the Expense Splitter Service project.

-----

# Expense Splitter Service

[cite\_start]A simple, single-page web application designed to help small groups like roommates or friends track shared expenses and easily figure out who owes whom[cite: 4]. [cite\_start]This application does all the math automatically, providing clear balances and the simplest way to settle up[cite: 8].

## Features

  - **Group Management**: Easily add members to an expense group.
  - [cite\_start]**Dynamic Expense Logging**: Record expenses with a description, amount, and specify who paid[cite: 14].
  - [cite\_start]**Flexible Splitting**: Select exactly which members of the group should share the cost for each expense[cite: 14].
  - [cite\_start]**Real-Time Balance Calculation**: The application automatically calculates and displays each member's running balance in real-time[cite: 15].
  - [cite\_start]**Optimized Settlements**: Generates a clear, minimal list of payments required to get everyone back to zero[cite: 12, 18].
  - **Responsive UI**: A clean, modern interface built with vanilla CSS that works on different screen sizes.

## How to Use

1.  **Add Group Members**:

      - In the "Add Member" panel, enter a name and click the **Add to Group** button.
      - Added members will appear as chips in the "Group Members" list.

2.  **Record an Expense**:

      - In the "Add Expense" panel, fill in the **Description** and **Amount**.
      - Select who **Paid By** from the dropdown menu of group members.
      - Under **Split Between**, check the boxes next to the names of all the people who are sharing this particular expense.

3.  **Submit the Expense**:

      - Click the **Record Expense** button.

4.  **Review the Summary**:

      - The expense will immediately appear in the "Recent Expenses" list.
      - [cite\_start]The "Balances" and "Settlements" panels will automatically update to reflect the new calculations[cite: 15].

## Installation

This is a standalone front-end application with no server-side dependencies or build steps required.

1.  **Download** the `index.html` file to your local machine.
2.  Open the `index.html` file directly in any modern web browser (e.g., Chrome, Firefox, Safari).

## Code Highlights

  - **HTML**: Provides the complete structure for the single-page application.
  - **CSS**: All styling is embedded within the HTML file for simplicity. It uses modern CSS properties like Grid for a responsive layout without any external frameworks.
  - **Vanilla JavaScript**: Powers all the dynamic functionality of the application. There are no external libraries or frameworks like jQuery or React.

### Key JavaScript Functions

  - `addMember()`: Adds a new person to the group, updating the UI and the underlying `members` array.
  - `addExpense()`: Validates and adds a new expense to the `expenses` array, then triggers updates across the UI.
  - `recalculate()`: The core function that is called after any change. It computes all balances from scratch and calls the functions to display balances and settlements.
  - `displayBalances()`: Renders the summary of what each person owes or is owed.
  - `displaySettlements()`: Implements a greedy algorithm to calculate the minimum number of transactions needed to clear all debts and displays them visually.

## Example Use Case

Imagine four roommates: Alice, Bob, Carol, and Dave.

  - Alice buys $100 worth of groceries for everyone. [cite\_start]She logs this expense, marking all four people as sharing it[cite: 9].
  - [cite\_start]Later, Bob pays a $60 utility bill that only covers his and Alice's rooms, so he enters this expense and includes only himself and Alice[cite: 10].
  - [cite\_start]The application automatically calculates the final balances and then shows the simplest way to settle up, such as "Carol pays Alice $10" and "Dave pays Bob $10"[cite: 11, 12].

## Screenshots

*(You can replace the placeholder URLs with actual screenshots of your application)*

**Main Application View:**

**Settlement View:**

## Technologies Used

  - HTML5
  - CSS3 (Flexbox & Grid)
  - Vanilla JavaScript

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
