# 🎯 JavaScript Event Handling & Interactive Elements Assignment

Welcome to the **ultimate JavaScript playground**! 🎉 This assignment is where we turn boring web pages into dynamic, responsive, *alive* experiences. Get ready to master **event handling**, build **interactive components**, and validate forms like a pro! 💪

## 📁 Assignment Structure

```
📂 js-event-assignment/
├── index.html         # Your playground – where it all comes together
├── style.css          # Keep it cute (optional but encouraged)
└── script.js          # The JavaScript wizardry happens here
```

---

## 🧪 What to Build

Here’s what your interactive bundle of joy should include:

### 1. Event Handling 🎈  
- Button click ✅  
- Hover effects ✅  
- Keypress detection ✅  
- Bonus: A secret action for a *double-click* or *long press* 🤫

### 2. Interactive Elements 🎮  
- A button that changes text or color  
- An image gallery or slideshow  
- Tabs or accordion-style content  
- Bonus: Add some animation using JS or CSS ✨

### 3. Form Validation 📋✅  
- Required field checks  
- Email format validation  
- Password rules (e.g., min 8 characters)  
- Bonus: Real-time feedback while typing

---

## 🧙‍♂️ Pro Tips

- Keep your code clean and commented – your future self will thank you!
- Think about **user experience** – what makes your site more *fun* to use?
- Don’t be afraid to **Google and experiment** – that’s how real developers roll!

---

## 🎉 Now Go Make It Fun!

Remember – this isn't just code. It's your **first step toward creating magical user experiences**. So play around, break stuff (then fix it), and most of all, have FUN! 😄

Happy Coding! 💻✨  

Event Handling:
We can use the addEventListener() method to attach event handlers to different elements on the page. For example, we can attach a click event handler to a button using the following code:
const button = document.getElementById("myButton");
button.addEventListener("click", function() {
  // Code to execute when the button is clicked
});
We can also use the mouseover and keydown events to create hover effects and detect keypress events.
2. Interactive Elements:
We can create a button that changes text or color by manipulating the innerHTML or style properties of the button element. For example, we can change the text of a button when it is clicked using the following code:
const button = document.getElementById("myButton");
button.addEventListener("click", function() {
  button.innerHTML = "New Text";
});
We can also create an image gallery or slideshow by manipulating the src attribute of an image element. For example, we can create a slideshow that cycles through a series of images using the following code:
const images = ["image1.jpg", "image2.jpg", "image3.jpg"];
let currentImage = 0;

const imageContainer = document.getElementById("imageContainer");
imageContainer.addEventListener("click", function() {
  currentImage++;
  if (currentImage >= images.length) {
    currentImage = 0;
  }
  imageContainer.innerHTML = `<img src="${images[currentImage]}" alt="Image">`;
});
We can also create tabs or accordion-style content by manipulating the style properties of the tab or accordion element. For example, we can toggle the visibility of a tab when it is clicked using the following code:
const tab = document.getElementById("myTab");
tab.addEventListener("click", function() {
  if (tab.style.display === "block") {
    tab.style.display = "none";
  } else {
    tab.style.display = "block";
  }
});
Form Validation:
We can use JavaScript to validate the input fields of a form before submitting the form. For example, we can check that a required field is not empty using the following code:
const form = document.getElementById("myForm");
form.addEventListener("submit", function(event) {
  const name = document.getElementById("name").value;
  if (name === "") {
    event.preventDefault();
    alert("Name is required");
  }
});
We can also validate the email format and password rules using regular expressions and other JavaScript methods.
4. Bonus: Real-time feedback while typing:
We can use JavaScript to manipulate the DOM and provide real-time feedback to the user while they are typing. For example, we can change the color of a form field based on whether it is valid or not using the following code:
const form = document.getElementById("myForm");
const name = document.getElementById("name");

form.addEventListener("input", function() {
  if (name.value === "") {
    name.style.color = "red";
  } else {
    name.style.color = "green";
  }
});
