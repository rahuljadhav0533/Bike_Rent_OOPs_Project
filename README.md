OOP Bike Rental System in Python
This project is a simple, full-fledged bike rental system implemented in Python using Object-Oriented Programming (OOP) principles. It demonstrates concepts like classes, objects, inheritance, and methods to manage a bike rental shop's inventory and customer transactions.

📋 Features
Stock Management: The shop starts with a predefined stock of bikes.
Customer Transactions: Customers can rent one or more bikes.

Flexible Rental Plans:
Daily Basis: Rent bikes for ₹100 per bike, per day.
Weekly Basis: Rent bikes for ₹500 per bike, per week.

Family Rental Discount: A special 30% discount is applied to the total bill if a customer rents between 3 and 5 bikes in a single transaction.

Real-time Inventory Check: The system checks for available stock before approving a rental request.

Billing: The system can generate a final bill when a customer returns the bikes.

🛠️ How It Works
The system is built around two main classes: BikeRental (the parent class) and Customer (the child class).

BikeRental Class
This class acts as the main shop.
It holds the total number of bikes available in stock (a class attribute).
The displaystock() method shows the current number of available bikes.

Customer Class
This class inherits from BikeRental and manages customer-specific actions.
When creating a Customer object, you specify the number of bikes, the rental basis ('day' or 'week'), and the duration.
The rentBike() method validates the request against available stock and updates the inventory.
The returnBike() method calculates the total bill based on the rental plan. It also checks if the customer is eligible for the family discount.
