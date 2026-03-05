Here is a "Starter Kit" you can give your students. It includes a deliberately messy HTML structure and a CSS file that is missing the Grid logic.

Your students' job is to **refactor** the HTML for accessibility and **apply** CSS Grid to create a professional layout.

---

### **Part 1: The "Broken" HTML (`index.html`)**

This code works, but it's "ugly" code. It lacks proper labeling, accessibility, and logical grouping.

```html
<form action="#">
  <h2>Join Apex Nebula</h2>
  
  <p>User Information</p>
  Username: <input type="text" name="user">
  Email: <input type="text" name="email"> Password: <input type="password" name="pass">

  <p>Class:</p>
  Warrior <input type="radio" name="class" value="warrior">
  Mage <input type="radio" name="class" value="mage">

  <p>Bio:</p>
  <textarea name="bio" placeholder="Tell us about yourself..."></textarea>

  <input type="checkbox" name="terms"> I agree to everything.
  
  <button>Go</button>
</form>

```

---

### **Part 2: The CSS Challenge (`style.css`)**

Give them this "reset" code. They must fill in the `@media` query and the `.form-grid` properties.

```css
/* Base Styles */
body {
  font-family: sans-serif;
  background: #121212;
  color: white;
  display: flex;
  justify-content: center;
  padding: 50px;
}

form {
  background: #1e1e1e;
  padding: 2rem;
  border-radius: 8px;
  width: 100%;
  max-width: 600px;
}

/* STUDENT TASK 1: Set up the Grid */
.form-group {
  display: grid;
  /* Hint: Use grid-template-columns for labels and inputs */
  gap: 1rem;
  align-items: center;
  margin-bottom: 1.5rem;
}

/* STUDENT TASK 2: Responsive Design */
@media (max-width: 600px) {
  .form-group {
    /* Hint: Change the grid layout for mobile */
  }
}

/* STUDENT TASK 3: Visual Feedback */
input:focus {
  /* Add a glow effect here */
}

```

---

### **How to Grade This**

When you review their work, look for these three specific "A-Ha!" moments:

1. **The Label Link:** Did they use `<label for="id">` and `<input id="id">`? If they click the text "Username" and the box highlights, they passed.
2. **The Grid Span:** Did they make the `<textarea>` or the `<h2>` span across both columns using `grid-column: 1 / -1;`?
3. **The Keyboard Trap:** Can they "Tab" through the form in a logical order?

