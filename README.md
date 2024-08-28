🗂️ Database Schema Overview

Our database schema in SQL is designed to manage and streamline car rentals. Below is an overview of the key tables and their purposes:
1. 🔐 UserCredentials

    Stores usernames and passwords for authentication purposes.
    Columns: Username, Password

2. 👤 Customers

    Holds detailed information about customers, including their names, emails, and phone numbers.
    Columns: CustomerName, CustomerEmail, CustomerPhone

3. 🚗 CarCategories

    Contains different categories of cars available for rent, with descriptions.
    Columns: CategoryName, CategoryDescription

4. 🚙 Cars

    Maintains details of the cars, such as brand, model, fuel average, seating capacity, status (available or rented), etc.
    Columns: CarBrand, CarModel, FuelAverage, SeatingCapacity, Status, LocationID, CarCategoryID

5. 🌍 Locations

    Stores location details, including city, state, and country, to track where cars are available.
    Columns: City, State, Country

6. 📅 Bookings

    Manages the rental bookings, linking customers with cars, including start and end dates.
    Columns: BookingID, CustomerID, CarID, BookingStartDate, BookingEndDate

7. 💳 Payments

    Tracks payment details for each booking, including amount, method, and status.
    Columns: PaymentID, BookingID, Amount, PaymentMethod, PaymentStatus

8. 👨‍💼 Employees

    Contains information about employees who manage the car rental services.
    Columns: EmployeeName, EmployeeEmail, EmployeePhone, JobTitle

9. 🏢 Branches

    Lists the physical branches of the car rental company, including their locations and contact details.
    Columns: BranchName, BranchLocation, BranchPhone

10. 🔧 Maintenance

    Keeps records of car maintenance schedules and details.
    Columns: CarID, MaintenanceDate, Details
