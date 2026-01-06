# josh_assignment_day_one

# Assignment One
# Database Technologies Used by Applications

## 1. Amazon – Amazon Aurora (Relational Database based on MySQL and PostgreSQL)

### Reasons:
- The data is in structured format like users, orders, payments, and invoices  
- There is a large number of transactions, so consistency is required; ACID properties in relational databases handle this well  
- Supports complex queries and joins across multiple tables  

---

## 2. LinkedIn – Espresso and LIquid

- **Espresso:** NoSQL document store for profiles  
- **LIquid:** Specialized graph database for connections  

### Reasons:
- LIquid efficiently stores connections and relationships and is easy to manage in graph form  
- Enables fast graph traversal for recommendations, as LinkedIn frequently needs to find new people in the network to connect with  

---

## 3. Uber – Redis and CacheFront

- **Redis:** In-memory database  
- **CacheFront:** Document store developed by Uber  

### Reasons:
- Data is stored in RAM for real-time access, making it faster  
- Supports sessions between riders and drivers  
- Works well because rider locations and other data need to be updated in real time  

---


# Assignment Three
# Database Normalization

## Why is normalization important?

**Answer:**

Normalization is the process of reducing data redundancy in a table and improving data integrity. It organizes data efficiently.

It is important because:

1. Normalization reduces redundancy, meaning data is not repeated, which results in smaller tables and is good for scaling.
2. We can write more efficient queries on normalized tables.
3. The relationships in the database are clearer, so we can manage them properly.
4. With normalization, we can avoid database anomalies.

---

## What problems occur if a database is not normalized?

**Answer:**

The problems that occur if the database is not normalized are:

1. Data duplication happens in the database, which causes more storage space to be used.
2. It causes different types of anomalies:
   - **Insertion anomalies:** We have to add unrelated data to insert valid data.
   - **Deletion anomalies:** Removing unrelated data can remove important data as well.
   - **Update anomalies:** We have to update many rows to change a single piece of data.
3. We are not able to scale the database properly.

---

## Convert the following unnormalized data into 1NF

### Unnormalized Table

| Order_ID | Customer_Name | Products        |
|---------:|---------------|-----------------|
| 101      | Rahul         | Laptop, Mouse   |

### Answer:

In 1NF, we cannot have multiple values in a single cell.

So, the table in **1NF** will look like this:

| Order_ID | Customer_Name | Products |
|---------:|---------------|----------|
| 101      | Rahul         | Laptop   |
| 102      | Rahul         | Mouse    |

*(Considering `Order_ID` as the primary key, it is kept unique.)*

