Certainly! Here's a concise README file for the branch addressing the diamond problem:

```markdown
# Solving the Diamond Problem in Python

## Diamond Problem Overview

Addressing the diamond problem in a class hierarchy involving `TemporarySecretary` class.

### Class Hierarchy

![Diamond Problem](https://files.realpython.com/media/ic-diamond-problem.8e685f12d3c2.jpg)

### Output Screenshot

![Output Screenshot](Capture4.PNG)

## Changes Made

Introduced the `TemporarySecretary` class, demonstrating the diamond problem in multiple inheritance and providing a solution through explicit method invocation.

### Example Usage

```python
import hr
import employees
import productivity

# ... (rest of the program setup)

temporary_secretary = employees.TemporarySecretary(5, 'Robin Williams', 40, 9)
company_employees = [
    manager,
    secretary,
    sales_guy,
    factory_worker,
    temporary_secretary,
]

# ... (rest of the program execution)
```

## Diamond Problem Resolution

Resolved the diamond problem by managing the order of inheritance and explicitly invoking methods.

### Code Snippet

```python
class TemporarySecretary(Secretary, HourlyEmployee):
    def __init__(self, id, name, hours_worked, hour_rate):
        HourlyEmployee.__init__(self, id, name, hours_worked, hour_rate)

    def calculate_payroll(self):
        return HourlyEmployee.calculate_payroll(self)
```

## Run the Program

Ensure Python is installed, then run:

```bash
python program.py
```

## Additional Resources

- [Understanding Python's Method Resolution Order (MRO)](https://realpython.com/python-method-resolution-order/)
- [Diamond Problem in Object-Oriented Design](https://en.wikipedia.org/wiki/Multiple_inheritance#The_diamond_problem)

Feel free to explore and experiment with the code.
```

Replace `<LINK_TO_CLASS_HIERARCHY_IMAGE>` with the actual URL where you can find the class hierarchy image.
