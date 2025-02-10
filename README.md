# CashRegister
# Cash Register App

## Project Overview
The **Cash Register App** is a JavaScript-based application that calculates and returns change based on the price of an item, the cash provided by the customer, and the available cash in the register. The app determines whether the transaction can be completed and displays the appropriate status.

## Features
- Input fields for **item price**, **customer cash**, and **available cash in the drawer (CID)**.
- Validation to ensure correct inputs.
- Automatic calculation of the required change.
- Three possible statuses:
  - **"OPEN"**: If there is enough cash to provide exact change.
  - **"CLOSED"**: If the change given depletes the register.
  - **"INSUFFICIENT_FUNDS"**: If exact change cannot be given.
- Breakdown of returned change in denominations.

## How It Works
1. The user enters the item price and the amount of cash given.
2. The app compares the values:
   - If the cash is **less than** the price → an alert is shown.
   - If the cash is **equal to** the price → "No change due" is displayed.
   - If the cash is **greater than** the price → the app calculates and returns change.
3. The app then checks the cash in the drawer (CID) and determines the transaction status based on available funds.

## Change Calculation
The app uses the following denominations to return change:
- $100 Bills
- $50 Bills
- $20 Bills
- $10 Bills
- $5 Bills
- $1 Bills
- $0.25 Quarters
- $0.10 Dimes
- $0.05 Nickels
- $0.01 Pennies

## Status Determination
- **"OPEN"**: If the register contains enough cash to return the exact change, the breakdown is displayed.
- **"CLOSED"**: If the exact change amount depletes the entire register.
- **"INSUFFICIENT_FUNDS"**: If the register does not have enough money or exact denominations to provide the required change.

## Technologies Used
- **HTML**: Provides the user interface for input fields and results.
- **CSS**: Styles the application layout.
- **JavaScript**: Implements the logic for handling transactions and change calculation.

## How to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/Ngila706/CashRegister.git
   ```
2. Open the `index.html` file in your browser.
3. Enter the required values and click the "Calculate Change" button.

## Future Improvements
- Add currency selection for international support.
- Implement a database to store past transactions.
- Improve UI with animations and better styling.

## License
This project is open-source under the MIT License.
