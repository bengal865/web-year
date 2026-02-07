# 🛠️ HTML5 Form Attributes: The Developer's Toolkit

Use these attributes to make your forms functional, accessible, and user-friendly.

---

### 1. The "Must-Haves" (Identification)
* **`id`**: The unique name for the element. Think of this as a "Social Security Number"—no two elements on a page should have the same ID. Essential for CSS styling and JavaScript.
    * *Example:* `<input id="user-email">`
* **`name`**: The label for the data sent to the server. If you don't have a `name`, the data doesn't exist when you hit Submit!
    * *Example:* `<input name="email_address">` → Results in `?email_address=user@test.com`

---

### 2. The "Rules" (Validation)
* **`required`**: A boolean attribute that prevents the form from submitting if the field is empty. The browser will show a warning automatically.
    * *Example:* `<input type="text" required>`
* **`readonly`**: The user can see the text and highlight it, but they cannot change it.
* **`disabled`**: The user cannot interact with the input at all, and the data is **not** sent when the form is submitted.

---

### 3. The "Experience" (Usability)
* **`placeholder`**: Temporary "ghost text" that shows a hint or example of what to type. It disappears as soon as the user starts typing.
    * *Example:* `<input placeholder="e.g. John Doe">`
* **`autocomplete`**: Helps the browser remember what the user typed before (like "name", "email", or "tel").
    * *Example:* `<input autocomplete="email">`
* **`autofocus`**: Automatically puts the cursor in this field as soon as the page loads.

---

### 4. The "State" (Selection)
* **`checked`**: Used for `radio` buttons and `checkboxes`. It makes the option "pre-selected" when the page loads.
    * *Example:* `<input type="checkbox" checked>`
* **`value`**: Defines the specific data sent to the server. For text inputs, it sets "default text." For buttons/radios, it defines the hidden data.
    * *Example:* `<input type="radio" value="yes">`

---

### 💡 Pro Tip: ID vs. Name
| Attribute | Who uses it? | Purpose |
| :--- | :--- | :--- |
| **`id`** | The Browser / CSS | Designing the look and targeting with JS. |
| **`name`** | The Server / URL | Identifying which "bucket" the data belongs in. |