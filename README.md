![image](https://github.com/user-attachments/assets/e2be68ad-abb9-4ccc-bca7-0f82856c27a0)

This project is a functional programming-based spreadsheet application written in JavaScript. It allows users to input mathematical expressions and apply built-in functions to data across cells. The core functionality involves parsing and evaluating expressions such as sums, averages, and custom-defined operations in a spreadsheet-like interface.

The infixToFunction object maps operators like +, -, *, and / to corresponding functions that perform arithmetic operations. The infixEval function takes a string representing a mathematical expression and applies the correct operation based on the operator, using regular expressions for parsing. The highPrecedence function ensures that multiplication and division are evaluated before addition and subtraction.

Additionally, the application supports a set of built-in spreadsheet functions, defined in spreadsheetFunctions. These include typical mathematical functions such as sum, average, median, as well as more specialized ones like even, random, and range. These functions are accessible within cell formulas, and can process values passed as comma-separated arguments.

The applyFunction function processes a string formula and evaluates it by replacing function calls with the results of the corresponding operations. It can also handle ranges of cells, defined with column-letter and row-number notation (e.g., A1:B2), by expanding these references into the corresponding values in the spreadsheet.

The evalFormula function processes complex formulas involving ranges and cell references, recursively expanding them and applying the appropriate functions to evaluate the result.

The front-end interface of the application dynamically generates a grid of cells, represented by input elements. These cells allow users to input data, and any formula prefixed with = will trigger the evaluation of the formula. The update function listens for changes in the input fields and automatically updates the cell values by evaluating the corresponding formulas.

Overall, this project combines functional programming principles with spreadsheet-like functionality, providing a highly customizable and dynamic way of evaluating expressions and formulas in a web-based interface.
