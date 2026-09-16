# SAVE THE BEAVERS !!!
 Save the Beavers - Charity E-Commerce Database

Welcome to my database implementation project. For this assignment, I designed "Save the Beavers", an associative e-commerce platform where purchases directly fund real-world conservation efforts. Instead of a standard retail store, this database tracks both financial transactions and the specific charitable impact of each purchase.

Database Architecture
The project relies on a relational schema consisting of 8 tables built in PostgreSQL:

* Core Transactions: The `Member` table stores donor information, while `Shop_Order` and `Order_Item` handle the purchases and specific quantities bought.
* Reference Tables: Each `Charity_Product` is categorized via the `Category` table and linked to a specific `Conservation_Project`. This structure ensures every item sold supports a defined cause.
* Weak Entities: To increase the realism of the model, I included two dependent tables with composite primary keys. `Shipping_Address` allows members to save multiple delivery locations, and `Inventory_Batch` manages stock levels across different incoming shipments.
