# SQL-Task8- Stored Procedures and Functions

## Objective
The goal of this task is to implement reusable SQL logic using stored procedures and functions in MySQL.

## What I Implemented

###  Tables Created
- `Customers`: Stores customer details
- `Orders`: Stores order information linked to customers

### Stored Procedure
- `GetOrdersByCustomer(IN cust_id INT)`: Fetches all orders by a specific customer ID

###  Function
- `CalculateBonus(amount DECIMAL(10,2))`: Returns 10% of the order amount as a bonus

## How to Use

 ###Procedure:

CALL GetOrdersByCustomer(1);

###Function:

SELECT OrderID, Amount, CalculateBonus(Amount) AS Bonus FROM Orders;
