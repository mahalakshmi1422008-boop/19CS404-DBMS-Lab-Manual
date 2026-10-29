# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
*Paste or attach your diagram here*  
<img width="1921" height="972" alt="image" src="https://github.com/user-attachments/assets/d1c5d3eb-49d0-47ac-8261-5b663eb5ad6e" />


### Entities and Attributes

| Entity | Attributes (PK, FK) |
|--------|--------------------|
|Customer    |1. CustomerID (Primary Key)2. Name3. ContactDetails4. TableNumber                    |       
|Waiter        |1. WaiterID (Primary Key)2. Name3. ContactDetails                   |       
|Chef       |1. ChefID (Primary Key)2. Name3. ContactDetails                    |       
| Table       |1. TableID (Primary Key)2. Location3. Status (e.g., occupied, available)                    |       
|FoodItem        |1. FoodItemID (Primary Key)2. Name3. Description4. Price5. Category (e.g., appetizer, main course, dessert)                    |  
| Order             | 1. OrderID (Primary Key)2. DateTime3. TotalAmount4. Status (e.g., pending, in preparation, completed, canceled)           |               
| OrderItem             | 1. OrderItemID (Primary Key)2. OrderID (Foreign Key)3. FoodItemID (Foreign Key)4. Quantity5. Status (e.g., ordered, being prepared, ready)           |               
|  Bill            |1. BillID (Primary Key)2. OrderID (Foreign Key)3. TotalAmount4. PaymentStatus (e.g., paid, unpaid)            |               
|Supervisor              |1. SupervisorID (Primary Key)2. Name3. ContactDetails            |                            

### Relationships and Constraints

| Relationship | Cardinality | 
|--------------|------------|
| MANAGES	             |One-to-Many            |               
| GENERATES	             |One-to-One            |               
| CREATES             | One-to-Many           |               
|SERVES              | Many-to-Many           |               
| CONTAINS	             |One-to-Many            |                 
| PREPARES	             |One-to-Many            |      
| REFERS TO	             | Many-to-Many           |               
| BELONGS TO             | Many-to-Many           |      
|HAS              |One-to-Many            |               


---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
