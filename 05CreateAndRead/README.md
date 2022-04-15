# Create and Readme

to start mongodb

```bash
mongo
```

to see all databases. this command will list all databases.

```bash
show dbs
```

**create database**
it will now change current database to books. it will not show now as db until it has at least one entry

```bash
use books
```

**Insert into database**
it will now change current database to client. it will not show now as db until it has at least one entry

```bash
db.bookData.insertOne({
    "name": "Make Habit",
    "author": "Nirav",
    "description":"nice book to read",
    "price":200,
    "isInEnglish":true
})
```

`findOne()` will list all data of document. or you can use `findOne().pretty()`

```bash
db.bookData.findOne()
```

mongodb converts json data into bson data and then saves.
saving BSON data is much more efficient as compare to JSON data.
[JSON and BSON](https://www.mongodb.com/json-and-bson)

we can also use key without using `""`.

```js
{
    name:"nirav",
    email:"n@n.com"
}
```
