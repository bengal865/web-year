## HTML Forms Intro / General Timeline

### Objective

By the end of this unit, students will be able to build a **responsive** web form using CSS Grid.

**NOTE:** The form will use various form input fields, including text and email fields, radio buttons, a drop-down list, etc., and form fields will be grouped using the `<legend>` and `<fieldset>` elements.

---

### Day 1: Introducing Web Forms

**Prompt:** Where have you filled out a form online recently? (Students provide examples)

**Key takeaway:** We use forms to collect info from users.

**Direct Instruction/Live Build:** 

- Absolute minimum HTML for page shell
- <form> element + <label> and <input type="text"> elements
- Use double <br> for spaces between <input> fields (no CSS)
- Use only <button type="submit">

1. <form> = container for user input
2. <label> + for attribute: Makes form accessible
3. type="email" --> for collecting email address specifically
4. Submit button --> Sends form data somewhere for processing

#### Student Work

- Build simple shipping form
  - First Name (text input)
  - Last Name (text input)
  - Email (email input)
  - Submit button 
- Use <label> element with `for` attribute correctly
- Only use double <br> to space out the input fields

**Required Files:** Unit 13 Proj 1 Instructions (.md), Unit 13 Proj 1 Basic Form (.html), Unit 13 Proj 1 Quick Start (.md)

#### Follow-Up Questions/Quick Check

1. What does the `<form>` element do?
2. Why use type="email" rather than type="text"?
3. What is the SUBMIT button used for?

### Day 2: Other Commonly Used Form Input Fields

**Focus:** 
- Compare good/bad form design (Which of these two forms is the more user-friendly form? **Why?**  (Provide specific examples))
- Add `action` and `method` attributes to Day 1 form
**Required Files:** Unit 13 Shipping Form Compare (.md), Unit 13 Shipping Form 1 (.html with TODOs), Unit 13 Forms Overview (.md), Unit 13 Proj 2 Exit (.md, already printed off), web-013-chk-html5-forms.md

### Day 3: Additional Form Field Attributes

- Yesterday: `action` and `method` attributes to Day 1 form
- **Today:** Add additional form input attributes (required, placeholder, maxlength)
- **Today:** How to apply a class to a specific <div>

**Required Files:** `web-u013-sol-shipping-form-part2.html` with TODO comments

**Focus:** 

- Discuss how you might use CSS Grid to make the form responsive
  - Why a 2-column layout?
  - How could we use grid template areas to map out the parts of the web form?
    - **Tie each template area name to a specific <div> class**
- Define grid template areas 
- What CSS Grid code is needed to make the form responsive?
- Introduce specs for media query also

### Day 4: Finish Building Responsive Web Form

**Demo:** Finished two-column responsive web form

#### CSS
- CSS Reset Rule
- `:root` element rule
- mobile-first template area map
- media query
- desktop template area map

**Required Files:** `web-u013-sol-shipping-form-part3.html`