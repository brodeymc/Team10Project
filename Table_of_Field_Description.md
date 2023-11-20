# **Table of Field Description**
Here you can find a description of every field and of every entity along with the data type:

## **Entity**: Product
| Field | Type | Default | Nullable | Relationship | Notes |
|-------|------|---------|----------|---------------|-------|
| ProductID | INT |  | NO | Primary Key | Unique identifier for each product. |
| Name | VARCHAR |  | NO |  | The name of the product. |
| Description | TEXT |  | YES |  | A detailed description of the product. |
| Price | DECIMAL | 0.00 | NO |  | The price of the product. |
| StockQuantity | INT | 0 | YES |  | The quantity of the product available. |
| CategoryID | INT |  | NO | Foreign Key to Category | Relates each product to a specific category. |

## **Entity**: Category
| Field | Type | Default | Nullable | Relationship | Notes |
|-------|------|---------|----------|---------------|-------|
| CategoryID | INT |  | NO | Primary Key | Unique identifier for each category |
| Name | VARCHAR |  | NO |  | The name of the category. |
| Description | TEXT |  | YES |  | A brief description of the category. |

## **Entity**: Customer
| Field | Type | Default | Nullable | Relationship | Notes |
|-------|------|---------|----------|---------------|-------|
| CustomerID | INT |  | NO | Primary Key | Unique identifier for each customer. |
| FirstName | VARCHAR |  | NO |  | The first name of the customer |
| LastName | VARCHAR |  | NO |  | The last name of the customer |
| Email | VARCHAR |  | NO |  | The email address of the customer |
| Address | TEXT |  | YES |  | The residential address of the customer. |
| PhoneNumber | VARCHAR |  | YES | Foreign Key to Category | The contact phone number of the customer. |

## **Entity**: Order
| Field | Type | Default | Nullable | Relationship | Notes |
|-------|------|---------|----------|---------------|-------|
| OrderID | INT |  | NO | Primary Key | Unique identifier for each order. |
| CustomerID | INT |  | NO | Foreign Key to Customer | Relates each order to a specific customer. |
| OrderDate | TIMESTAMP | CURRENT_TIMESTAMP | NO |  | The date and time when the order was placed. |
| TotalAmount | DECIMAL | 0.00 | NO |  | The total amount of the order. |
| Status| VARCHAR | 'Processing' | NO |  | The status of the order. |



