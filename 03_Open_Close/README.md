# Open Close Principle

- Class should be Open for Extension but Closed for Modification.

### Bad Implementation :

- Below EmployeeSalary class calculates salary based on employee type: Permanent and Contractual.

- Issue: In the future, if a new type (Part-time Employee) comes then the code needs to be modified to calculate the salary based on employee type.

```cpp
public class EmployeeSalary {

    public long calculateSalary(Employee emp) {
        Long salary = null;

        if 
    }
}

```