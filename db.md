

## database

> **database**: A file composed of records, each containing fields together with a set of operations for searching, sorting, recombining, and other functions. 

database 的缩略写法为 db.

[例句][1]：

> The following example will demonstrate how a web page can fetch information from a database with AJAX.

[再比如][2]：

> **Creating a Database**
To create a database in MySQL, use the "CREATE DATABASE" statement:

```
var mysql = require('mysql');

var con = mysql.createConnection({
  host: "localhost",
  user: "yourusername",
  password: "yourpassword"
});

con.connect(function(err) {
  if (err) throw err;
  console.log("Connected!");
  con.query("CREATE DATABASE mydb", function (err, result) {
    if (err) throw err;
    console.log("Database created");
  });
});
```

---

【补充】： db 同时也是`decibel`的缩写：分贝
> **decibel**：a unit for measuring the loudness of sound.

例句：
> Continuous exposure to sound above 80 **decibels** could be harmful. 

[1]: https://www.w3schools.com/js/js_ajax_database.asp
[2]: https://www.w3schools.com/nodejs/nodejs_mysql_create_db.asp
