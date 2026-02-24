# Optical Practice Data Extraction

## 📌 Project Overview
This project simulates a real-world task: extracting historical transaction data from a database for a client using "My Vision Express" (optical software). I built a sample SQLite database with patients, orders, products, and order items, then wrote SQL queries to extract meaningful transaction data.

## 🛠️ Skills Demonstrated
- SQL (CREATE, INSERT, SELECT, JOIN)
- Database design and schema understanding
- Data extraction and export to CSV
- Working with foreign keys and relationships

## 📂 Files Included
- `optical_transactions.csv` – the extracted transaction data
- `extract_transactions.sql` – the SQL query used (optional)
- `database_schema.sql` – the full script to build the database (optional)

## 🔍 SQL Query Used
```sql
SELECT 
    orders.order_id,
    orders.order_date,
    patients.first_name || ' ' || patients.last_name AS patient_name,
    products.product_name,
    order_items.quantity,
    order_items.price_per_item,
    (order_items.quantity * order_items.price_per_item) AS line_total,
    orders.status
FROM orders
JOIN patients ON orders.patient_id = patients.patient_id
JOIN order_items ON orders.order_id = order_items.order_id
JOIN products ON order_items.product_id = products.product_id
ORDER BY orders.order_date;
...
order_id,order_date,patient_name,product_name,quantity,price_per_item,line_total,status
1,2023-11-15,John Smith,Single Vision Lenses,2,89.99,179.98,Completed
1,2023-11-15,John Smith,Anti-Reflective Coating,1,45.0,45.0,Completed
2,2023-11-28,Mary Johnson,Ray-Ban Aviator,1,150.0,150.0,Completed
3,2023-12-05,John Smith,Progressive Lenses,1,249.99,249.99,Completed
4,2023-12-12,Robert Williams,Oakley Holbrook,1,135.0,135.0,Completed
4,2023-12-12,Robert Williams,Transition Lenses,1,110.0,110.0,Completed
5,2024-01-03,Patricia Brown,Single Vision Lenses,1,89.99,89.99,Completed
5,2024-01-03,Patricia Brown,Anti-Reflective Coating,1,45.0,45.0,Completed
6,2024-01-18,Mary Johnson,Ray-Ban Aviator,2,150.0,300.0,Pending
7,2024-01-22,Michael Jones,Progressive Lenses,1,249.99,249.99,Completed
8,2024-02-10,John Smith,Single Vision Lenses,1,89.99,89.99,Processing
8,2024-02-10,John Smith,Transition Lenses,1,110.0,110.0,Processing
9,2024-02-14,Robert Williams,Oakley Holbrook,1,135.0,135.0,Completed
