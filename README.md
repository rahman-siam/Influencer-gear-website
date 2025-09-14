# JavaScript DOM & Event Questions

## 1. Difference between `getElementById`, `getElementsByClassName`, and `querySelector / querySelectorAll`

- **`getElementById(id)`**  
  - Returns a single element with the specified `id`.  
  - Example: `document.getElementById('myId')`  

- **`getElementsByClassName(className)`**  
  - Returns a live HTMLCollection of all elements with the specified class.  
  - Example: `document.getElementsByClassName('myClass')`  

- **`querySelector(selector)`**  
  - Returns the **first element** matching the CSS selector.  
  - Example: `document.querySelector('.myClass')`  

- **`querySelectorAll(selector)`**  
  - Returns a **static NodeList** of all elements matching the CSS selector.  
  - Example: `document.querySelectorAll('.myClass')`  

---

## 2. How to create and insert a new element into the DOM

```javascript
// 1. Create a new element
const newDiv = document.createElement('div');
newDiv.textContent = "Hello, I'm new!";

// 2. Select parent element
const parent = document.getElementById('parentDiv');

// 3. Insert new element
parent.appendChild(newDiv);  // Adds at the end
// or
parent.insertBefore(newDiv, parent.firstChild); // Adds at the beginning
