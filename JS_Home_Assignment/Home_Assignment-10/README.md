
# Day10Homework

This is a simple HTML and JavaScript code that changes the background color of the webpage when the button is clicked.

Hosted Link : https://hackerbubai007.github.io/Module-6_JS_Home_Assignment/JS_Home_Assignment/Home_Assignment-10/index.html

### HTML Code

The HTML code consists of a `<div>` element that contains a button. The button has an `onclick` event listener that calls the `changeBackgroundColor()` function when clicked.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Day10Homework</title>
</head>
<body>
    <div>
        <button>Change BackGroundColor</button>
    </div>
    
</body>
</html>
```

### JavaScript Code

The JavaScript code consists of a single function called `changeBackgroundColor()`. This function changes the background color of the webpage by setting the `backgroundColor` property of the `body` element.

```javascript
var Color = [
    "green",
    "cyan",
    "black",
    "voilet",
    "blue",
    "yellow",
    "purple",
    "orange",
    "lightgreen",
    "lemon",
  ];
  var index = 0 ;
  var div = document.querySelector("div");
  const button = document.querySelector("button");
  button.addEventListener("click", function() {
      if (index === Color.length) {
          index = 0;
    }
          div.style.backgroundColor = Color[index];
          index++;
  })
```
