initDB(): This function initializes the database and creates two tables, “accounts” and “expenses,” if they don’t exist. It uses SQLite as the database engine.

addAccount(String accountName): This function adds an account to the database. It takes the account name as input and inserts it into the “accounts” table.

loadData(DefaultTableModel model, int acId): This function loads expense data from the database into the JTable component. It clears the existing table data, retrieves expense data for the specified account ID, and populates the table using a DefaultTableModel.

getAccountDetails(int accountId): This function retrieves account details such as account name and total expense amount from the database. It executes SQL queries to fetch the required data and returns the details as an array.

addExpense(int accountId, String date, String description, double amount): This function adds an expense to the currently selected account. It takes the account ID, date, description, and amount as input and inserts them into the “expenses” table.

updateCombox(JComboBox<String> cbx): This function updates the JComboBox component with account data from the database. It clears the existing items and retrieves account data from the “accounts” table, adding them as items to the combo box.

initialize(): This function initializes the GUI components of the Expense Tracker application. It sets up the frame, panels, labels, text fields, table, and buttons, along with their respective event listeners.


These functions work together to provide functionality for adding accounts, selecting accounts, adding expenses, and displaying account details and expense data in the GUI.