# Ans to the qn no: 01

## 1. getElementById()

Used to select an element by its ID.
Always returns only one element (the one with that ID).

Example:
```javascript
<span id="icon"></span>
document.getElementById("icon");

```

## 2. getElementsByClassName()

Used to select multiple elements by their class name.Returns an HTMLCollection of all matching elements.

Example:
```javascript
<span class="icon"></span>
<span class="icon"></span>
document.getElemenstByClassName("icon");

```

## 3. querySelector()

Used to find the first element that matches a given selector. It returns the first matching element.

Example:
```javascript
<span class="icon"></span>
<span class="icon"></span>
document.querySelector(".icon");

```

## 4. querySelectorAll()

 Returns a NodeList of all elements that match the given selector.

Example:
```javascript
<span class="icon"></span>
<span class="icon"></span>
document.querySelectorAll(".icon");

```

# Ans to the qn no: 02

1.Create a new element using document.createElement().
2.Add content to the element using textContent or innerHTML.
3.Select the parent element where to insert.
4.Insert the new element using appendChild().

Example:

```javascript
const newElement = document.createElement("div"); 
newElement.textContent = "New DOM!";
newElement.setAttribute("id", "newDiv");  
document.body.appendChild(newElement);     

```


