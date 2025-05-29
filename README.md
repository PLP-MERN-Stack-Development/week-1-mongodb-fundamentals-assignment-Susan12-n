# MongoDB Bookstore Scripts

This project contains MongoDB queries and aggregation pipelines for managing and analyzing data in a `books` collection.

---

##  Prerequisites

-  MongoDB installed locally or access to a MongoDB Atlas cloud cluster
- Mongo Shell (`mongosh`) or MongoDB Compass
- A collection named `books` with fields such as:
  - `title` (string)
  - `author` (string)
  - `genre` (string)
  - `published_year` (number)
  - `price` (number)
  - `in_stock` (boolean)

---

##  How to Run the Scripts

###  1. Open the Mongo Shell

**Local MongoDB:**

```bash
mongosh

---


##  📂 2. Switch to the Correct Database 

-use bookstore

---

 # 3. Run Queries

 ```js
db.books.aggregate([
  { $group: { _id: "$genre", avgPrice: { $avg: "$price" } } }
])

---

 ### sreenshots

 ![compass images](images/image1.png.png)
 ![compass images](images/image2.png.png)








