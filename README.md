
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

## **Query Commands**

| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | db.mycollection.find() | retrieves all the documents in the collection |
| 2. | db.mycollection.find().pretty() | retrieves all the documents in an easy-to-read format  |
| 3. | db.mycollection.findOne({name: "by"}) | retrieves all the documents having name "by" |
| 4. | db.mycollection.find({$and:[{"name":"by"},{"lang": "eng"}]}).pretty() | it show all data having name 'by' and whose lang is 'eng'. |
| 5. | db.mycollection.find({$or:[{"name":"by"},{"lang": "eng"}]}).pretty() | it show all data having name 'by' or lang is 'eng'  |

## **Limiting records**

| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | db.mycollection.find({},{"name":1,"lang":0}).limit(1) | show only one record |
| 2. | db.mycol.find({},{"name":1,"lang":0}).limit(1).skip(1) | skip first and fetch next one |

## **Sorting records**

| **Sno.** | **Command** | **Command Do** |
| ---- | ------- | ---------- |
| 1. | db.collection.find().sort({id:1}) | sort record in Ascending |
| 2. | db.collection.find().sort({id:-1}) | sort record in Descending |
