# VB Auto Center

## Overview
The VB Auto Center is a simple Windows Forms application developed in VB.NET that calculates the total price of a car, considering the base price, trade-in value, selected accessories, and the finish type. It also computes the sales tax and displays the final amount due after applying the trade-in value.

## Features
- **Base Price and Trade-in Validation**: Ensures that the base price is greater than 0 and the trade-in value is non-negative.
- **Accessory Selection**: Users can select additional options for the car, including stereo, leather interior, and navigation system.
- **Finish Type**: The application allows users to select between a pearlized or custom car finish.
- **Sales Tax Calculation**: The tax is calculated at a rate of 8% based on the base price and selected accessories.
- **Total Calculation**: The program calculates and displays the subtotal, tax, and the final amount due after subtracting the trade-in value.

## Constants
- **Stereo Price**: $500
- **Leather Price**: $1,000
- **Navigation Price**: $1,500
- **Pearlized Finish Price**: $500
- **Custom Finish Price**: $750
- **Tax Rate**: 8% (0.08)

## Program Flow
1. **Input Validation**: The program checks if the base price and trade-in values are numeric and valid.
2. **Accessory and Finish Calculation**: Based on user selection, the program adds the cost of selected accessories (Stereo, Leather, Navigation) and the chosen finish (Pearlized or Custom).
3. **Tax Calculation**: The program calculates the sales tax at 8% of the base price plus the selected accessories.
4. **Subtotal Calculation**: The subtotal is calculated by adding the base price, accessories cost, and tax.
5. **Final Amount Due**: The final amount due is calculated by subtracting the trade-in value from the subtotal.
6. **Display Results**: The results, including accessory price, subtotal, tax, and final amount due, are displayed in the user interface.

## Controls and Methods

### `btnClear_Click`
- Clears all input fields, selections, and output labels, resetting the trade-in value to 0.

### `btnCalc_Click`
- Validates user input and performs the car price calculation (base price, accessories, tax, subtotal, final amount due).
- Calls validation and calculation methods to ensure proper inputs and computations.

### `Get_Validate_Input`
- Validates the base price and trade-in value.

### `Get_Validate_Base_Price`
- Ensures the base price is numeric and greater than 0.

### `Get_Validate_Trade`
- Ensures the trade-in value is numeric and non-negative.

### `Calculate_Car_Price`
- Calls helper methods to calculate the price, including accessories, finish, tax, and final total.

### `Calculate_AF_Price`
- Calculates the price for accessories and finish.

### `Calculate_Accessories`
- Adds the price of selected accessories (Stereo, Leather, Navigation).

### `Calcuate_Finish`
- Adds the price for the selected finish type (Pearlized or Custom).

### `Calculate_Tax`
- Calculates the tax as 8% of the sum of base price and accessories.

### `Calculate_SubTotal`
- Calculates the subtotal by adding the base price, accessories, and tax.

### `Calcluate_Total`
- Subtracts the trade-in value from the subtotal to get the final amount due.

### `Display_Totals`
- Displays the accessory price, tax, subtotal, and amount due in the UI.

### `btnExit_Click`
- Closes the application.

## How to Use
1. Enter the **Base Price** of the car in the designated field.
2. Enter the **Trade-in** value (if applicable).
3. Choose the accessories you would like to add: **Stereo**, **Leather**, **Navigation**.
4. Select the **Finish Type** (either **Pearlized** or **Custom**).
5. Click **Calculate** to compute the price.
6. Review the calculated price, including accessories, tax, and the final amount due after the trade-in.
7. Click **Clear** to reset all fields and selections.
8. Click **Exit** to close the application.

## Example
**Inputs:**
- **Base Price**: $25,000
- **Trade-in**: $2,000
- **Accessories**: Stereo, Leather, Navigation
- **Finish**: Custom

**Output:**
- **Accessory Price**: $3,000 (Stereo + Leather + Navigation)
- **Tax**: $2,240 (8% of $25,000 + $3,000)
- **Subtotal**: $30,240
- **Amount Due**: $28,240 (After $2,000 trade-in)

## Requirements
- .NET Framework
- Visual Studio or any VB.NET compatible IDE


