# Lesson 1: Introduction to MongoDB

---

## 📘 What is a Database?

- An **organized collection of data** - in the simplest terms.  
- It provides methods to **manipulate and manage** data efficiently.

---

## 🍃 What is MongoDB?

- **MongoDB** is a **NoSQL database** that stores data in a **flexible, JSON-like format**.  
- It makes it easy to **scale** and handle **large volumes of unstructured data**.  
- Data in MongoDB is stored in:
  - **Collections** → groups of related documents  
  - **Documents** → individual JSON-like records within a collection  

---

### 🧩 Basic Structure

| SQL Term       | MongoDB Equivalent |
|----------------|--------------------|
| Table          | Collection         |
| Row            | Document           |
| Column         | Field              |

- A **field** is a key-value pair within a document (like a column in SQL).  
- A **document** can also contain **nested (embedded) documents**, meaning one document inside another.

---

### 💡 Real-Life Example

Think of a **Library System**:
- A **collection** → “Books”
- Each **document** → one book’s details (title, author, genre, etc.)
- **Fields** → individual attributes like “Title”, “Author”, “ISBN”
- Some fields (like “Author Details”) can be **embedded documents**, e.g.:
  ```json
  {
    "title": "Python for Data Analysis",
    "author": {
      "name": "Wes McKinney",
      "country": "USA"
    },
    "published_year": 2022
  }

# ⚖️ SQL vs NoSQL

---

## 1. Scalability

- **NoSQL:** Scales **horizontally** by adding more servers and distributing the load across multiple nodes.  
- **SQL:** Scales **vertically** by adding more resources (CPU, RAM) to a single server - this has limits and can be costly.  
- **Sharding** (splitting data across servers) is more complex and less efficient in SQL.

---

## 2. Schema Flexibility

- **NoSQL:** Schema-less design - supports diverse and rapidly changing data structures **without altering schema**.  
- **SQL:** Requires a **predefined schema**. Altering it (e.g., adding new columns) is **complex and time-consuming**, especially with large datasets.

---

## 3. Performance

- **NoSQL:** Ideal for **real-time data processing and analytics**, with **high-speed read/write operations**.  
- **SQL:** Can be slower with large data volumes due to **rigid schema** and **complex joins**.

---

## 4. Handling Unstructured Data

- **NoSQL:** Efficiently handles **semi-structured** and **unstructured data**.  
- **SQL:** Best suited for **structured data**, stored in a tabular format with predefined attributes.

---

## 🧠 Summary

**MongoDB** provides **flexibility**, **scalability**, and **performance** for modern data workloads - making it perfect for projects involving **unstructured** or **fast-changing data**.
