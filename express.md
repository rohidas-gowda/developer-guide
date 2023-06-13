> **NPM Package**

<br />

```
npm i express
```

<br />

> **Express Boilerplate**
```javascript
const express = require('express')
const app = express()

// respond with "hello world" when a GET request is made to the homepage
app.get('/', (req, res) => {
  res.send('hello world')
})

app.listen(1337, () => {
    console.log('Server started on 1337')
})
```
<br />

> **CORS & JSON Middleware**
```javascript
const express = require('express')
const cors = require('cors')
const app = express()

app.use(cors())
app.use(express.json())

// respond with "hello world" when a GET request is made to the homepage
app.get('/', (req, res) => {
  res.send('hello world')
})
```
