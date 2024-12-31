Food Production Automation System
This project aims to automate the production line in a food manufacturing plant, starting from the process of purchasing raw materials and ending with the finished products entering the warehouse. The system integrates with various departments such as Purchasing, Inventory Management, Production, Sales, and Quality Control.

Features
Raw Materials Management: The system tracks the raw materials required for each product, manages inventory levels, and handles orders from the purchasing department.
Production Process: Each product passes through several stages, or machines, where raw materials are consumed and processed. The production process tracks machine capacity and raw material consumption.
Warehouse Management: Finished products and raw materials are stored in specific warehouses, each responsible for a particular type of material or product. The system manages the minimum and maximum inventory levels for each product.
Product Specifications: Each product has specific details such as production date, expiration date, wholesale price, and retail price.
Quality Control: Products that fail quality control are moved to a special warehouse for discounted sale.
Sales Management: Sales reduce the inventory of finished products, and the system tracks this process to ensure accurate stock levels.
Alerts and Notifications: The system generates alerts for inventory levels that fall below or exceed defined limits in the warehouse.
Technologies Used
Database Management System: Oracle Database for storing raw material, product, and warehouse data.
Programming Languages: SQL for database queries and procedures, C# for application logic and database interaction.
Production Line: The system automates processes such as raw material consumption, product manufacturing, and product storage in warehouses.
ERD (Entity-Relationship Diagram): A detailed ERD is designed to show how the database entities are related, ensuring efficient data flow across departments.
Project Components
1. Raw Materials Management
Each product requires specific quantities of raw materials, which are purchased by the Purchasing Department.
Raw materials are stored in different warehouses, with each warehouse dedicated to storing specific raw materials.
The system tracks the inventory levels of raw materials and issues alerts when the stock goes below the minimum or exceeds the maximum threshold.
2. Production Process
The system monitors the production process, where raw materials are consumed as products pass through various machines (or workstations).
Each machine has a daily production capacity, and the system calculates the necessary raw materials based on the production volume.
When a product exits a machine, the system consumes the required amount of raw materials.
The finished product is then moved to a warehouse, updating the warehouse stock.
3. Product Management
Each product has a set of specifications, including production date, expiration date, wholesale price, and retail price.
Products that fail the Quality Control Department are moved to a special warehouse for discounted sale.
4. Inventory Management
The system maintains the current stock levels of both raw materials and finished products.
Inventory levels are continuously updated as raw materials are consumed in production, and products are sold.
Alerts are generated when inventory levels are out of range (either too high or too low).
5. Sales Management
Sales Department processes sales transactions, which reduce the finished product inventory.
The system tracks sales and adjusts inventory in real-time.
6. HR System Integration
The system is integrated with the Human Resources (HR) system to manage employees working on the production line and monitor work hours.
Database Design
ERD (Entity-Relationship Diagram)
The ERD visualizes the relationships between key entities such as Raw Materials, Products, Machines, Warehouses, Purchasing, Production, Sales, and Quality Control. Each entity has attributes, and the relationships between them ensure smooth operations across departments.

Database Procedures and Functions
Create Tables with Constraints: SQL scripts are used to create the necessary tables and enforce integrity constraints.
Production Procedure: A stored procedure calculates the quantity of raw materials required to produce a specific quantity of a product. The procedure ensures sufficient stock is available and raises an error if raw materials are insufficient.
Work Hour Calculation Function: A function is designed to calculate the number of work hours required to produce a specific quantity of a product based on machine capacity.
Inventory Alert Trigger: A trigger is implemented to alert when the quantity of a product or raw material in the warehouse goes below the minimum or exceeds the maximum allowed stock level.
