# Firebase Database Easily
Módulo que facilita a entrada e saída de informações pelo Firebase Realtime Database

# Conexão
```js
const FDE = require("fireabse-database-easily")
const database = new FDE.connection("API-KEY", "AUTH-DOMAIN", "DATABASE-URL", "PROJECT-ID", "STORAGE-BUCKET", "MESSAGING-SENDER-ID", "ID")
```

# Método SET
```js
database.set(`Users/${id}/Test`, {information: "yes", information2: "not"})
```

# Método UPDATE
```js
database.update(`Users/${id}/Test`, {information: "omg!", FDE: "cool"})
```

# Método GET (once)
```js
database.get(`Users/${id}/Test`, information).then(information => console.log(information)) //omg!
```

# Firebase
Configure seu database acessando o [Console do Firebase](https://console.firebase.google.com)
