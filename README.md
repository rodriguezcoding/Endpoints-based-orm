# Endpoints-based-orm

## Client example:

```javascript
let socket = io.connect("server url");
socket.on("orm.js", data => {
  eval(data.apiOrm);
  console.log(data.functionNames)
  find({token:"some auth token here", params:["param value here"]}).then(data=>console.log(data))
});
```
