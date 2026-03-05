# 🛠️ Form Fixer-Upper: Worksheet

**Name:** ________________________  
**Date:** _________________________

### Task: Identify and fix the errors in the following code snippets.

---

## 1. The Accessibility Gap 🧩
**The Goal:** When the user clicks the word "Username," the input box should become active. 
**The Problem:** Currently, clicking the label does nothing.

```html
<label for="user-field">Username</label>
<input type="text" name="username">

```

**What is the fix?**

---

---

## 2. The Keyboard Sabotage ⌨️

**The Goal:** A user is signing up on their iPhone. You want the keyboard to automatically show the `@` symbol when they tap the email field.
**The Problem:** The current code just shows a standard alphabet keyboard.

```html
<label for="email">Email Address</label>
<input type="text" id="email" name="user_email">

```

**What is the fix?**

---

---

## 3. The "Grid Area" Disconnect 🗺️

**The Goal:** The student wants the button to sit in the specific "button" area defined in their `grid-template-areas` map.
**The Problem:** The button is ignoring the grid map and floating randomly.

**CSS:**

```css
.field-container {
    display: grid;
    grid-template-areas: 
        "label-user  input-user"
        ".           submit-zone";
}

```

**HTML:**

```html
<button class="btn-main">Create Account</button>

```

**What CSS rule is missing to link the button to the "submit-zone"?**

---

---

## 4. The Data Guard 🛡️

**The Goal:** You want to make sure the user enters at least 10 characters for their "Player Bio" and that they cannot leave it blank.

**HTML:**

```html
<label for="bio">Bio</label>
<textarea id="bio" name="bio"></textarea>

```

**Which two attributes should you add to the `<textarea>` tag to enforce these rules?**

1.

-----
2.

-----

---

### 💡 Answer Key for Teacher:

1. **Fix:** Add `id="user-field"` to the `<input>` tag so it matches the label's `for` attribute.
2. **Fix:** Change `type="text"` to `type="email"`.
3. **Fix:** Add `.btn-main { grid-area: submit-zone; }` to the CSS.
4. **Fix:** `required` and `minlength="10"`.

