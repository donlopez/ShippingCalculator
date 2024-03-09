# Shipping Calculator

## Overview

The Shipping Calculator is a console-based application written in C++ that calculates the shipping cost of a package based on its weight (in pounds) and the distance it will travel (in miles). This user-friendly application supports calculating shipping costs for packages up to 10 pounds over any distance.

## Features

- **User Input**: Captures user input for the number of miles and the weight of the package in pounds.
- **Input Validation**: Ensures miles and package weight inputs are valid (greater than zero and within the weight limit).
- **Cost Calculation**: Dynamically calculates the shipping cost based on package weight and travel distance.
- **Session Continuity**: Allows users to calculate shipping costs for multiple packages in a single session.

## How It Works

### Functions

- `milesToSegment(int)`: Validates that the input for miles is greater than zero. This function sets the stage for further enhancements, like segment-based rate calculations.
- `twopounds(int, double)`: Calculates shipping cost for packages up to 2 pounds.
- `twoToSixpounds(int, double)`: Calculates shipping cost for packages over 2 pounds and up to 6 pounds.
- `sixToTenpounds(int, double)`: Calculates shipping cost for packages over 6 pounds and up to 10 pounds.

Each function calculates the shipping cost based on the distance (divided into 500-mile segments) and the package's weight category. The cost calculation takes into account the entire segment if there's a remainder in the mileage division, ensuring accurate cost estimation.

### Main Workflow

1. Prompt the user to enter the shipping distance in miles and validate this input.
2. Request the package weight in pounds, ensuring it falls within the supported range.
3. Determine the applicable cost calculation function based on the package weight.
4. Display the calculated shipping cost to the user.
5. Offer the user an option to calculate the shipping cost for another package or exit the program.

## Compilation and Execution Instructions

To compile the program, use a C++ compiler with the following command:

```bash
g++ -o shipping_calculator shipping_calculator.cpp
./shipping_calculator

Sample Usage:

Enter the number of Miles as a whole number: 1200
Enter the Weight of the package in pounds: 4
The cost to ship your package is: $14.80

Enter 1 to continue or 0 to quit: 0

Good-bye!


This markdown text is ready to be included in a `README.md` file and uploaded to GitHub, providing a structured and informative description of the Shipping Calculator project, including how to compile and run the program.
