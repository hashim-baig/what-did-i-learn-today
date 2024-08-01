# Adding JavaScript files to HTML

- ## Writing JavaScript inside Head Tag

```index.html

<!DOCTYPE html>
<html>
    <head>
        <title>JavaScript</title>
        <script>
            alert("JavaScript Loaded");
        </script>
    </head>
    <body>
    
    </body>
</html>

```


- ## Writing JavaScript in another file

```index.html

<!DOCTYPE html>
<html>
    <head>
        <title>JavaScript</title>
        <script src="./script.js"></script>
    </head>
    <body>
    
    </body>
</html>

```

```script.js

alert("JavaScript Loaded")

```
