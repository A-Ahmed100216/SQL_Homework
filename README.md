# SQL Querying Homework
## 1.  How many orders in NWDB?
* **Query**
```sql
SELECT COUNT(*) FROM Orders
```
* **Response**   
**830**

## 2. How many orders are there where the Ship City is Rio de Janeiro?
* **Query**
```sql
SELECT COUNT(*) FROM Orders where ShipCity='Rio de Janeiro'
```
* **Response**   
**34**   

## 3. Select all orders that the Ship City is Rio de Janeiro or Reims?
* **Query**
```sql
SELECT OrderID,ShipCity FROM Orders where ShipCity='Rio de Janeiro' or ShipCity='Reims'
```
* **Response**   
**39 orders**

![q3](https://github.com/A-Ahmed100216/SQL_Homework/blob/main/Images/q3.png)

## 4. Select all of the entries where the Company name has a z or a Z in the table of Customers.
* **Query**
```sql
SELECT * FROM Customers WHERE CompanyName LIKE '%Z%' or CompanyName LIKE '%z%'
```
* **Response**    
**6 instances where z appears in a company name.**
![q4](https://github.com/A-Ahmed100216/SQL_Homework/blob/main/Images/q4.png)

## 5. Find me the Name of All of the companies that do not have FAX numbers! I would also like to know with whom I need to speak with, their contact numbers and what city they are based in.
* **Query**
```sql
SELECT CompanyName, ContactName, Phone, City  FROM Customers WHERE Fax IS NULL
```
* **Response**   
![q5](https://github.com/A-Ahmed100216/SQL_Homework/blob/main/Images/q5.png)

## 6. Ahh there you are! My prize ⭐⭐SPARTANTS⭐⭐! MY MARES AND MY STALLIONS! We need to re-target all of our Customers is Paris! Get me information on these clients.
* **Query**
```sql
SELECT *  FROM Customers WHERE City='Paris'
```
* **Response** 
![q6](https://github.com/A-Ahmed100216/SQL_Homework/blob/main/Images/q6.png)

## 7. WAIT! Where are you going? (...) These clients are hard to sell too! We need more intel.. Can you find out, from these clients from Paris, whom orders the most by quantity? Who are our top 5 clients?
* **Query**
```sql
SELECT TOP 5 * FROM [Order Details] ORDER BY Quantity DESC
```
* **Response**
![q7](https://github.com/A-Ahmed100216/SQL_Homework/blob/main/Images/q7.png)

## 8. I need to know more about these these Paris client. Can you find out which ones their deliveries took longer than 10 days? Display the Business/client name, contact name, all their contact details (don't forget the fax!), as well as the number of deliveries that where overdue! Just add a column named: 'Number overdue orders'
* **Query**
```sql

```
* **Response**
![q8]()


