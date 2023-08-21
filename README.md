# Console-Finances

Here's a breakdown of what the code does:

1. Initialize variables:
   - `average`: To store the calculated average change.
   - `analysis`: To store the analysis result.
   - `months`: The number of months in the `finances` array.
   - `total`: To calculate the total profit/loss.
   - `change`: To calculate the change in profit/loss for each month.
   - `net`: To keep track of the net profit/loss.
   - `netArray`: An array to store the individual changes for later calculations.
   - `netChangeSum`: To calculate the sum of all changes.
   - `least`: An array to store the month with the greatest decrease in profit.
   - `greatest`: An array to store the month with the greatest increase in profit.

2. Loop through the `finances` array using two nested loops:
   - The outer loop iterates through each element of the array.
   - The inner loop iterates through the sub-elements of each month.

3. Calculate various metrics:
   - Calculate the `total` profit/loss by adding up the values.
   - Calculate the `change` in profit/loss between the current month and the previous month.
   - Add the `change` to the `netArray`.
   - Update the `net` profit/loss for the next iteration.
   - Determine if the current `change` is the greatest increase or decrease, updating `greatest` and `least` arrays accordingly.

4. Calculate the `average` change by summing up all the changes in the `netArray` and dividing by the number of months.

5. Construct the `analysis` string using template literals to display the calculated metrics.

6. Output the `analysis` result to the console.

![Screenshot](./images/Screenshot%202023-08-21%20at%203.49.45%20AM.png)

The code essentially processes the provided financial data and outputs a summary of financial analysis metrics. It calculates the total, average change, and identifies the months with the greatest increase and decrease in profit.