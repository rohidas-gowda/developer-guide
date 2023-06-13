>MongoDB Connection

```javascript
const mongoose = require("mongoose");

mongoose.connect("mongodb://0.0.0.0:00000/<database-name>");

```

>Create Mongoose Model

```javascript
const mongoose = require("mongoose");

const Schema = mongoose.Schema;

let product = new Schema({
  name: String,
  price: Number,
  inStock: Boolean,
});

const model = mongoose.model("products", product);

module.exports = model;
```

>Access Mongoose Model in Express Router

```javascript
const mongoose = require('mongoose')

const Product = require("./models/product.model");

app.post("/api/product", async (req, res) => {
  try {
    await Product.insertMany({
      name: req.body.name,
      price: req.body.price,
      inStock: req.body.inStock,
    });
    res.json({ status: "ok" });
  } catch (error) {
    res.json({ status: "error", error: "duplicate product info" });
  }
});
```

>MongoDB CRUD Operations

>create documents:
```javascript
db.collection.insertOne()
db.collection.insertMany()
```

>read documents:
```javascript
db.collection.findOne()
db.collection.find()
```

>update documents:
```javascript
db.collection.updateOne()
db.collection.updateMany()
```

>delete documents:
```javascript
db.collection.deleteOne()
db.collection.deleteMany()
```
