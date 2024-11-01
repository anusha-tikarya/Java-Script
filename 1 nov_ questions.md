## 1
```html 
<!DOCTYPE html>
<html>
<head>
    <title>Select a Color</title>
</head>
<body>
    <h1>Select a Color</h1>
    <select id="colorSelect" onchange="showSelectedColor()">
        <option value="">--Choose a color--</option>
        <option value="Red">Red</option>
        <option value="Green">Green</option>
        <option value="Blue">Blue</option>
        <option value="Yellow">Yellow</option>
    </select>

    <script>
        function showSelectedColor() {
            alert('You selected: ' + document.getElementById('colorSelect').value);
        }
    </script>
</body>
</html>
```
## 2
```html
<!DOCTYPE html>
<html>
<head>
  <title> Onload Question </title>
</head>
</html>
<body onload = "pageloadedAlert()">
<script>
  function pageloadedAlert(){
  alert("Page loaded! ");
  }
  
</script>

</body>
</html>
```

```
## 2
