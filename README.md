# Udhaar App

Udhaar App- Buy-now-Pay-later is a command-line application that helps users manage credit transactions and track dues. It allows users to create new users and merchants, perform transactions, update discounts, and generate reports.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/udhaar-app.git
   ```

2. Navigate to the project directory:
   ```
   cd udhaar-app
   ```

3. Install dependencies:
   ```
   go mod download
   ```

4. Set up the database:
   - Ensure MySQL is installed and running on your system.
   - Create a new database named `udhaar_db`.
   - Import the database schema from the `database/schema.sql` file.

5. Configure the database connection:
   - Open the `database/db.go` file.
   - Modify the MySQL connection settings according to your configuration.

6. Build the application:
   ```
   go build
   ```

7. Run the application:
   ```
   ./udhaar-app
   ```

## Usage

The Udhaar App supports the following commands:

1. Add User: Create a new user account.
   ```
   add user <name> <phone_number> <credit_limit>
   ```

2. Add Merchant: Create a new merchant account.
   ```
   add merchant <name> <discount>
   ```

3. Update Merchant: Update the discount offered by a merchant.
   ```
   update merchant <name> <new_discount>
   ```

4. New Transaction: Perform a new credit transaction.
   ```
   new txn <user_email> <merchant_name> <amount>
   ```

5. Payback: Make a payment to reduce user dues.
   ```
   payback <user_email> <amount>
   ```

6. Report Discount: Get the discount offered by a merchant.
   ```
   report discount <merchant_name>
   ```

7. Report Dues: Get the dues of a specific user.
   ```
   report dues <user_email>
   ```

8. Report Users at Credit Limit: Get a list of users whose dues are equal to their credit limit.
   ```
   report users-at-credit-limit
   ```

9. Report Total Dues: Get the total dues across all users.
   ```
   report total-dues
   ```

## Constants

The application uses the following constants:

- Reset: ANSI escape code for resetting text formatting.
- Red, Green, Yellow, Blue, Purple, Cyan, Gray, White: ANSI escape codes for colored text.
- UdhaarAppSymbol: ASCII art symbol representing the Udhaar App.

## Error Messages

The application defines several error messages for different scenarios, such as invalid commands, credit limit exceeded, invalid input, missing data, and more.

## Database

The application uses a MySQL database to store user, merchant, and transaction data. The database schema is defined in the `database/schema.sql` file.

## Project Structure

The project follows a layered architecture, with the following main directories:

- `cmd`: Contains the main application logic.
- `constants`: Defines constants and error messages.
- `layer`: Implements the business logic and data logic of the application.
- `models`: Contains the data models used in the application.
- `utils`: Provides utility functions for input validation and formatting.
- `database`: Handles the database connection and operations.
- `repo`: Implements the repository layer for database interactions.

Feel free to explore the code in these directories for more details.

## Contributing

Contributions are welcome! If you find any issues or want to add new features, please create a pull request or submit an issue on GitHub.

##
# Udhaar App

Udhaar App is a command-line application that helps users manage credit transactions and track dues. It allows users to create new users and merchants, perform transactions, update discounts, and generate reports.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/udhaar-app.git
   ```

2. Navigate to the project directory:
   ```
   cd udhaar-app
   ```

3. Install dependencies:
   ```
   go mod download
   ```

4. Set up the database:
   - Ensure MySQL is installed and running on your system.
   - Create a new database named `udhaar_db`.
   - Import the database schema from the `database/schema.sql` file.

5. Configure the database connection:
   - Open the `database/db.go` file.
   - Modify the MySQL connection settings according to your configuration.

6. Build the application:
   ```
   go build
   ```

7. Run the application:
   ```
   ./udhaar-app
   ```

## Usage

The Udhaar App supports the following commands:

1. Add User: Create a new user account.
   ```
   add user <name> <phone_number> <credit_limit>
   ```

2. Add Merchant: Create a new merchant account.
   ```
   add merchant <name> <discount>
   ```

3. Update Merchant: Update the discount offered by a merchant.
   ```
   update merchant <name> <new_discount>
   ```

4. New Transaction: Perform a new credit transaction.
   ```
   new txn <user_email> <merchant_name> <amount>
   ```

5. Payback: Make a payment to reduce user dues.
   ```
   payback <user_email> <amount>
   ```

6. Report Discount: Get the discount offered by a merchant.
   ```
   report discount <merchant_name>
   ```

7. Report Dues: Get the dues of a specific user.
   ```
   report dues <user_email>
   ```

8. Report Users at Credit Limit: Get a list of users whose dues are equal to their credit limit.
   ```
   report users-at-credit-limit
   ```

9. Report Total Dues: Get the total dues across all users.
   ```
   report total-dues
   ```

## Constants

The application uses the following constants:

- Reset: ANSI escape code for resetting text formatting.
- Red, Green, Yellow, Blue, Purple, Cyan, Gray, White: ANSI escape codes for colored text.
- UdhaarAppSymbol: ASCII art symbol representing the Udhaar App.

## Error Messages

The application defines several error messages for different scenarios, such as invalid commands, credit limit exceeded, invalid input, missing data, and more.

## Database

The application uses a MySQL database to store user, merchant, and transaction data. The database schema is defined in the `database/schema.sql` file.

## Project Structure

The project follows a layered architecture, with the following main directories:

- `cmd`: Contains the main application logic.
- `constants`: Defines constants and error messages.
- `layer`: Implements the business logic and data logic of the application.
- `models`: Contains the data models used in the application.
- `utils`: Provides utility functions for input validation and formatting.
- `database`: Handles the database connection and operations.
- `repo`: Implements the repository layer for database interactions.

Feel free to explore the code in these directories for more details.

## Contributing

Contributions are welcome! If you find any issues or want to add new features, please create a pull request or submit an issue on GitHub.

## License

This project is licensed under the [MIT License](LICENSE).

---

Thank you for using Udhaar App! If you have any questions or need assistance, please feel free to contact us.
