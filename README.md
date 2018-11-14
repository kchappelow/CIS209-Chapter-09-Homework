# CIS209 Chapter 9 Homework

In this chapter, you studied an inheritance hierarchy in which class BasePlusCommissionEmployee inherited from class CommissionEmployee. 

However, not all types of employees are CommissionEmployees. In this exercise, you’ll create a more general Employee superclass that factors out the attributes and behaviors in class CommissionEmployee that are common to all Employees. 

The common attributes and behaviors for all Employees are 
* firstName, 
* lastName, 
* socialSecurityNumber, 
* getFirstName, 
* getLastName, 
* getSocialSecurityNumber 
* and a portion of method toString. 

Create a new superclass Employee that contains these instance variables and methods and a constructor. 

Next, rewrite class CommissionEmployee from Section 9.4.5 as a subclass of Employee. 

Class CommissionEmployee should contain only the instance variables and methods that are not declared in superclass Employee. Class CommissionEmployee’s constructor should invoke class Employee’s constructor, and CommissionEmployee’s toString method should invoke Employee’s to-String method. 

Once you’ve completed these modifications, run the EmployeeTest app using these new classes to ensure that the apps still display the same results for a CommissionEmployee object and BasePlusCommissionEmployee object, respectively.

Next, create a new class HourlyEmployee that inherits from class Employee and has instance variables
 * hours (a double) that represents the hours worked, 
 * wage (a double ) that represents the wages per hour, 

The HourlyEmployee should have a constructor that takes as arguments 
* a first name, 
* a last name, 
* a social security number, 
* an hourly wage and the 
* number of hours worked

It should have 
* set and get methods for manipulating the hours and wage, 
* an earnings method to calculate an HourlyEmployee’s earnings based on the hours worked
* toString method that returns the HourlyEmployee’s String representation. 

Method setWage should ensure that wage is nonnegative, and setHours should ensure that the value of hours is between 0 and 168 (the total number of hours in a week). 

Update the EmployeeTest class to use HourlyEmployee as well as CommissionEmployee and BasePlusCommissionEmployee.

Submit the new classes and modifications using git.
