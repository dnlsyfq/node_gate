### Setting 

```
$npm init
$npm install
$npm install express
$npm install ejs
$node app.py
```

### Routing

Request to particular url

Each route can handle a request with a function, known as a route handler

app.get('/top',(req,res) => {
    res.render('top.ejs');
});

### Create Page

app_project
|_app.js
|_views
|   |_top.ejs
|

### CSS , Image folder
path relative to public

public\css\style.css
public\images\top.png

```
// app.js
app.use(express.static('public'));

// html
<link href="/css/style.css">


<img src="/images/top.png">
```
