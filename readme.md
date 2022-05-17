
# **MongoDB Cheet Sheet**
- MongoDB is an open-source document-oriented database.
- It is categorized under the NoSQL database.
- MongoDB is written in C++
- The MongoDB database is developed and managed by MongoDB.Inc under SSPL(Server Side Public License) and initially released in February 2009.



## **Database Commands**

| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | show dbs | To show all databases|
| 2. | use dbname | To create or switch database |
| 3. | db | To view current database |
| 4. | db.dropDatabase() | For Delete database |


## **Collection Commands**

| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | show collections | To show Collection |
| 2. | db.createCollection('mycollection') | create new collection |
| 3. | db.mycollection.drop() | for drop collection |


## **Row Commands**


| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | db.mycollection.insertone({'name': 'bunny', 'lang': 'eng', 'id': 5}) | Insert One Row |
| 2. | db.mycollection.insertMany([{'name': 'by', 'lang': 'eng', 'id': 2 }, {'name': 'maker', 'lang': 'eng', 'id': 3 }]) | Insert Many Row |
| 3. | db.mycollection.remove({'name':'by'}) | remove all the documents whose name is 'by' |

