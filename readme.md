# Entrenamiento Scrum

> - https://gh.fgp.one/notes/scrum/auth/001front-login
> - https://gh.fgp.one/notes/scrum/auth/002front-register

```js
const express = require("express");
const app = express();
const port = 3000;

app.get("/", (req, res) => {
  res.send("Hello World!");
});

app.listen(port, () => {
  console.log(`Example app listening at http://localhost:${port}`);
});
```
