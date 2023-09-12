# Node JS

Node heavily uses async programming, hence there are a lots of callbacks used.
Callbacks were older ways of writing async code now use of promices are used.

## Install express which is lightweight web framework
```python
npm init
npm install express
```

## Use express

```javascript

const express = require("express")

const app = express()

app.get("/", (req, res)=>{
    res.send("Hello World");
});

app.listen(process.env.port || 3000, ()=>console.log("App running at http://localhost:3000"));
```

require was used to import packadges in older node versions now import is used insted.
