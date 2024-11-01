<img width="960" alt="{2102B8E1-65AC-4253-8D00-5D0E03D2D017}" src="https://github.com/user-attachments/assets/7c1aba59-172e-4a6f-b2c2-b61a43d63549">

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


## 3
```html
<!DOCTYPE html>
<html>
<head>
  <title> OnClick Question </title>
</head>
</html>
<body>
<button onclick="changeText(this)">click me</button>
<script>
  function changeText(button){
  button.innerHTML = "Clicked";
  }
  
</script>

</body>
</html>
```

## 4
```html
<!DOCTYPE html>
<html>
<head>
    <title>Onkeypress Count</title>
</head>
<body>
    <input type="text" onkeypress="countKeyPresses()" id="inputField">
    <p>Key Press Count: <span id="keyCount">0</span></p>

    <script>
        let count = 0;

        function countKeyPresses() {
            count++;
            document.getElementById("keyCount").innerHTML = count;
        }
    </script>
</body>
</html>
```
## 5
```html
<!DOCTYPE html>
<html>
<head>
    <title>OnkeyUP Question</title>
</head>
<body>
    <input type="text" onkeypress="displayUpperCase()" id="textInput">
    <p>displayUppercase Text: <span id="uppercaseText"></span></p>

    <script>


        function displayUpperCase() {
            let inputText = document.getElementById("textInput").value;
            document.getElementById("uppercaseText").innerHTML = inputText.toUpperCase();
        }
    </script>
</body>
</html>
```
