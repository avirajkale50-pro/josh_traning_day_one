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
