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
 
