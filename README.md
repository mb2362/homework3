# Intermediate Calculator

This project is an intermediate-level calculator that utilizes static methods on the `Calculator` class and instance methods on the `Calculation` class to perform arithmetic operations.

## Project Structure
```
calculator/
│── __init__.py
│── calculation.py
│── operations.py
│── tests/
    │── test_calculations.py
    │── test_calculator.py
```

## Installation
1. Clone this repository:
   ```sh
   git clone <repository_url>
   cd calculator
   ```
2. Install dependencies (if required):
   ```sh
   pip install -r requirements.txt
   ```

## Usage
The calculator provides four basic arithmetic operations:
- Addition
- Subtraction
- Multiplication
- Division

### Example Usage
```python
from calculator import Calculator

result_add = Calculator.add(5, 3)        # Returns 8
result_subtract = Calculator.subtract(5, 3)  # Returns 2
result_multiply = Calculator.multiply(5, 3)  # Returns 15
result_divide = Calculator.divide(6, 3)  # Returns 2.0
```

## Project Files
### `__init__.py`
- Imports modules and defines the `Calculator` class with static methods to perform operations.

### `calculation.py`
- Defines the `Calculation` class, which stores numbers and an operation function.
- Uses the `get_result` method to execute the stored operation.

### `operations.py`
- Defines functions for basic arithmetic operations: `add`, `subtract`, `multiply`, `divide`.

### `tests/test_calculations.py`
- Unit tests for the individual arithmetic functions in `operations.py`.

### `tests/test_calculator.py`
- Unit tests for the `Calculator` class methods.

## Running Tests
To run the test suite, use:
```sh
pytest tests/
```
Ensure `pytest` is installed:
```sh
pip install pytest
```