Here is a mini-project prompt designed to challenge their CSS Grid skills while enforcing the "Vital 20%" of form development.

---

## Project Prompt: The "Level Up" Registration Portal

### **The Scenario**

A new indie gaming platform, **Apex Nebula**, needs a responsive user registration page. They want a "pro-tier" experience that looks sleek on a 27-inch monitor but remains fully functional on a smartphone.

### **The Requirements**

Your form must include the following technical components:

#### **1. Semantic Structure**

* Use a single `<form>` wrapper with a logical `action` (e.g., `#`) and `method="POST"`.
* Group user data into two `<fieldset>` sections: **Account Details** and **Gaming Preferences**.
* Every input **must** have a corresponding `<label>` using the `for` attribute.

#### **2. The "Vital" Inputs**

* **Text & Email:** Username and Email fields (ensure `type="email"` is used).
* **Password:** A password field with a `minlength="8"` requirement.
* **Radio Buttons:** A "Choose Your Hero Class" section (Warrior, Mage, or Rogue).
* **Checkbox:** A "Sign up for the newsletter" and "Agree to Terms of Service" (Required).
* **Select Menu:** A "Region" dropdown (North America, Europe, Asia, etc.).

#### **3. The CSS Grid Layout**

* **Desktop View:** Use a 2-column grid where labels sit to the left of their inputs.
* **Mobile View:** Use a media query to stack the labels on top of the inputs for better readability on small screens.
* **Visual Feedback:** Use the `:focus` pseudo-class to change the border color or add a subtle box-shadow when a user clicks into a field.

---

### **Success Criteria (The Checklist)**

| Feature | Mastery Level |
| --- | --- |
| **Accessibility** | Can I click the text label to toggle the checkbox or focus the input? |
| **Validation** | Does the browser stop me if I leave a "Required" field blank? |
| **Responsiveness** | Does the form "snap" from 2 columns to 1 column at 600px width? |
| **UX Design** | Are the buttons clearly defined and the spacing consistent? |

---

### **Bonus Challenge**

Add a "Profile Bio" using a `<textarea>` that limits the user to 200 characters and uses CSS Grid’s `grid-column: span 2;` to make it take up the full width of the form on desktop.

