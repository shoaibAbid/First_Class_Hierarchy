<!DOCTYPE html>
<html lang="en">

<body>

  <h1>Employee Payroll System</h1>

  <p>This project serves as an illustrative example of class hierarchies in Python, showcasing the implementation of an HR system designed for payroll processing. The system employs the concept of inheritance to model different types of employees.</p>

  <h2>Class Hierarchy</h2>

  <p>The project defines a class hierarchy with a base class, <code>Employee</code>, and several derived classes, including <code>SalaryEmployee</code>, <code>HourlyEmployee</code>, and <code>CommissionEmployee</code>. Each derived class provides a specific implementation of the <code>calculate_payroll()</code> method, allowing for flexibility and customization based on employee type.</p>

  <img src="https://files.realpython.com/media/ic-initial-employee-inheritance.b5f1e65cb8d1.jpg" alt="Class Hierarchy">

  <h2>Implementation Overview</h2>

  <p>The heart of the system lies in the <code>Employee</code> base class, which encapsulates common attributes shared among all employee types. The derived classes extend this base, introducing specialized attributes and behaviors.</p>

  <p>The <code>PayrollSystem</code> class orchestrates the payroll calculation process. It iterates through a collection of employees, leveraging their specific <code>calculate_payroll()</code> methods to determine individual compensation.</p>

  <h2>Example Usage</h2>

  <p>To demonstrate the system in action, consider the following Python script:</p>

  <pre><code>import hr

# Create instances of different employee types
salary_employee = hr.SalaryEmployee(1, 'John Smith', 1500)
hourly_employee = hr.HourlyEmployee(2, 'Jane Doe', 40, 15)
commission_employee = hr.CommissionEmployee(3, 'Kevin Bacon', 1000, 250)

# Initialize the PayrollSystem
payroll_system = hr.PayrollSystem()

# Calculate payroll for the given employees
payroll_system.calculate_payroll([
    salary_employee,
    hourly_employee,
    commission_employee
])
</code></pre>

  <h2>Output</h2>

  <p>The system generates output in the terminal, providing insights into the calculated payroll for each employee. A placeholder for the output screenshot is provided below:</p>

  <p>[Output Screenshot Placeholder]</p>
  <img src="Capture1.PNG" alt="Output Screenshot">

</body>

</html>
