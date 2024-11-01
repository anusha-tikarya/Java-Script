<img width="960" alt="{8F98D4DB-4E5E-4C50-A1F1-CDFA80007764}" src="https://github.com/user-attachments/assets/1695f3e3-0a07-404d-8e1c-0b68723d0cd5">

<img width="960" alt="image" src="https://github.com/user-attachments/assets/76499184-de80-459a-9175-35fd2fbd3126">

<img width="960" alt="{68258C46-B88B-428C-9EB3-A61C9252C370}" src="https://github.com/user-attachments/assets/f559ea3b-0b61-4808-b9e5-7ba5ed545d25">
## find nodes
web page -- root node -- document
<img width="960" alt="{B082B019-CCF7-4F1B-B3B8-1F8E5ED626BA}" src="https://github.com/user-attachments/assets/222a0c57-dfc5-4e5d-b9d5-2eeb69ee4dc1">
1. getElementById()
2. getElementByClassName()
3. getElementByTagName()
4. querySelector()
5. querySelectorAll()

## dom manipulation
<img width="960" alt="{17B7C19F-0D8B-42B4-8DAF-A37550300996}" src="https://github.com/user-attachments/assets/4f257539-2b42-4581-869b-c808d4c02cc2">
```html
<!DOCTYPE html>
<html>
<head>
    <title>Sample</title>
</head>
<body>
    <p id="example">This is a Original product</p>
    <button onclick="changeText()">ADD TO CART</button>
    <script>
        function changeText(){
            alert("added to cart")
            document.getElementById("example").textContent = "Product added to the cart"
        }
    </script>
</body>
</html>
 ```
<img width="960" alt="{A34D09A4-15E9-4306-9CC9-EFFD345CB12E}" src="https://github.com/user-attachments/assets/ba5d87a8-fe7c-408d-b4ae-1ff7362f2ff7">

```html
<!DOCTYPE html>
<html>
<head>
    <title>Sample</title>
</head>
<body>
    <p id="example">This is a Original product</p>
    <button onclick="changeText()">ADD TO CART</button>
    <script>
        function changeText(){
            document.getElementById("example").textContent = "Product added to the cart";
            document.getElementById("example").style.color = "blue";
            document.getElementById("example").style.fontSize = "30px";
            document.getElementById("example").style.backgroundColor = "yellow";
        }
    </script>
</body>
</html>
```
## ***********************************************************
```html
<!DOCTYPE html>
<html>
<head>
    <title>Sample</title>
</head>
<body>
    <p id="example">This is a Original text.</p>
    <button onclick="changeText()">Change Text</button>
    <script>
        function changeText(){
            alert("CHANGING THE TEXT")
        }
    </script>
</body>
</html>
has context menu
```

# -----------------------------------------------
```html
<!DOCTYPE html>
<html>
<head>
    <title>Sample</title>
</head>
<body>
    <div id="container">
        <p>Para-1</p>
    </div>
    <button onclick="addParagraph()">Add Paragraph</button>
 
    <script>
        function addParagraph(){
            var newpara = document.createElement("p");
            newpara.textContent = "Para-2";
 
            document.getElementById("container").appendChild(newpara);
        }
    </script>
</body>
</html>
``` 
 ##  add------------------
```html
<!DOCTYPE html>
<html>
<head>
    <title>Sample</title>
</head>
<body>
    <div id="container">
        <p>Para-1</p>
    </div>
    <button onclick="addParagraph()">Add Paragraph</button>
 
    <script>
        function addParagraph(){
            var newpara = document.createElement("p");
            newpara.textContent = "Para-2";
 
            document.getElementById("container").appendChild(newpara);
 
            var third = document.createElement("h1");
            third.textContent= 'This is the Heading1';
            document.getElementById("container").appendChild(third);
        }
    </script>
</body>
</html>
 ```
## - -----------------
<img width="960" alt="{1909C1A5-A8BA-49CB-85C4-5DB9633E42A8}" src="https://github.com/user-attachments/assets/ca2e09ce-ce4a-4a00-a1c9-cc806dda1837">
```html
<!DOCTYPE html>
<html>
<head>
<title>Sample</title>
</head>
<body>
<div id="container">
<p id="removablepara">This para will be removed</p>
</div>
<button onClick="addParagraph()">Add Para</button>
<button onclick="removeLastParagraph()">Remove Last Para</button>
 
<script>
    function addParagraph(){
        var para = document.createElement("p");
        para.textContent = "Para-1";
        document.getElementById("container").appendChild(para);
    }
 
    function removeLastParagraph(){
        var container = document.getElementById("container");
        var paragraphs = container.getElementsByTagName("p");
        if (paragraphs.length > 0) {
            container.removeChild(paragraphs[paragraphs.length - 1]);
        }
    }
</script>
</body>
</html>
```
.
.
.
.

<img width="960" alt="{0FEA265D-FFC2-4064-B912-856887171CAF}" src="https://github.com/user-attachments/assets/4df8b89f-d06d-43af-8e59-4fc6f90d0ea5">


<img width="960" alt="{8C2F9325-4BBE-4034-A74B-2200CA5A656D}" src="https://github.com/user-attachments/assets/64dd01cb-b0f2-48f3-8b6a-f21e71d902c1">
```html
<!-- <!DOCTYPE html>
  <html>
  <head>
      <title>Sample</title>
  </head>
  <body>
    <div class="container">
       <p class="example">Para-1</p>
    </div>
    <button onclick="addPara()">Add Para</button>
   
      <script>
          function addPara(){
              var newpara = document.createElement("p");
              newpara.className = "example";
              newpara.textContent = "this is new para";
 
              document.getElementsByClassName("container")[0].appendChild(newpara);
 
          }
      </script>
  </body>
  </html> 
  
 ```html
  <!DOCTYPE html>
  <html>
  <head>
      <title>Sample</title>
  </head>
  <body>
    <div id="container">
        <p class="example">Para-1</p>
        <p class="example">Para-2</p>
    </div>
    <button onclick="removePara()">REMOVE PARA</button>
   
      <script>
          function removePara(){
            var elements = document.getElementsByClassName("example");  
           
            elements[0].remove();
           
          }
      </script>
  </body>
  </html>
```
<img width="960" alt="{CBB0D38E-8E5B-495D-9A78-BCDA82C4523F}" src="https://github.com/user-attachments/assets/2131bd43-8a91-4d1d-ae2d-c1ca7711aa0f">

<img width="960" alt="{C914E830-ACA2-4971-8EE4-DDAA8B0E7F5C}" src="https://github.com/user-attachments/assets/db0e01c2-051f-4f0b-9cda-fa61612dc7bd">


```html
<!DOCTYPE html>
<html>
<head>
    <title>DOM Manipulation with querySelector</title>
</head>
<body>
    <p>Look at my style change for paragraph 1!</p>
    <p>Look at my style change for paragraph 2!</p>
    <button onclick="changeStyle()">Change Style</button>
 
    <script>
        function changeStyle() {
            // Accessing the first paragraph and updating its style
            var paragraph = document.querySelector("p");
            paragraph.style.color = "blue";
            paragraph.style.fontSize = "20px";
            paragraph.style.backgroundColor = "yellow";
        }
    </script>
</body>
</html>
```
