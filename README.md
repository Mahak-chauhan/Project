# Dynamic Color Boxes

This project creates an animated visual of multiple vertically aligned boxes that continuously change their background and text colors at random intervals. It is built using HTML, CSS, and JavaScript.

## 🌐 Demo

Each box changes color independently, creating a colorful and engaging display. Great for learning about:

- DOM manipulation
- Random RGB color generation
- `setInterval` usage
- Flexbox layout

## 📁 Files

- `index.html` — Main HTML structure containing 25 `.box` elements inside a flex container.
- `style.css` — (Internal within `index.html`) Contains styling for the flex layout and box dimensions.
- `script.js` — JavaScript logic to apply random colors at intervals to each box.

## 🚀 How It Works

1. The page creates 25 box divs styled to be tall and narrow.
2. JavaScript selects all child elements of the container.
3. Each box is assigned two `setInterval` functions:
   - One for changing the background color.
   - One for changing the text color (though no text is currently present).

### Color Generator Function

```js
function getrandomcolor(){
    let var1 = Math.ceil(Math.random() * 255);
    let var2 = Math.ceil(Math.random() * 255);
    let var3 = Math.ceil(Math.random() * 255);
    return `rgb(${var1}, ${var2}, ${var3})`;
}
