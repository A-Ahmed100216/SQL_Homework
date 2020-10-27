# SQL Querying Homework
## 1.  How many orders in NWDB?
* **Query**
```sql
SELECT COUNT(*) FROM Orders
```
* **Response: 830**

## 2. How many orders are there where the Ship City is Rio de Janeiro?
* **Query**
```sql
SELECT COUNT(*) FROM Orders where ShipCity='Rio de Janeiro'
```
* **Response: 34 **

## 3. Select all orders that the Ship City is Rio de Janeiro or Reims?
* **Query**
```sql
SELECT OrderID,ShipCity FROM Orders where ShipCity='Rio de Janeiro' or ShipCity='Reims'
```
* **Response: 39 orders  **

![q3]()

## 4. Select all of the entries where the Company name has a z or a Z in the table of Customers.
* **Query**
```sql
SELECT * FROM Customers WHERE CompanyName LIKE 'Z%' or CompanyName LIKE '%z'
```
* **Response: There are zero instances of 'z' or 'Z' appearing in the company name.   **

## 5. Find me the Name of All of the companies that do not have FAX numbers! I would also like to know with whom I need to speak with, their contact numbers and what city they are based in.
* **Query**
```sql
SELECT CompanyName, ContactName, Phone, City  FROM Customers WHERE Fax IS NULL
```
* **Response:*   
![q5]()

## 6. Ahh there you are! My prize ⭐⭐SPARTANTS⭐⭐! MY MARES AND MY STALLIONS! We need to re-target all of our Customers is Paris! Get me information on these clients.
* **Query**
```sql
SELECT *  FROM Customers WHERE City='Paris'
```
* **Response:* 
![q6]()
