
# Quiz: HTML5 Forms and Field Attributes

**Name:** ___________________________  
**Date:** ___________________________

---

### Part 1: Multiple Choice (2 Points Each)

**1. Which attribute specifies the URL where the form data should be sent after submission?**
   - A) method
   - B) name
   - C) action
   - D) target

**2. Which attribute is used to group related options within a drop-down select list?**
   - A) <fieldset>
   - B) <optgroup>
   - C) <group>
   - D) <section>

**3. What is the default value of the 'method' attribute if it is not explicitly defined?**
   - A) POST
   - B) SEND
   - C) SUBMIT
   - D) GET

**4. Which attribute must be included on an input tag for the server to recognize and process the data?**
   - A) id
   - B) name
   - C) class
   - D) placeholder

**5. For a login form containing a password, which method is the most secure to use?**
   - A) GET
   - B) POST
   - C) ACTION
   - D) HIDDEN

**6. Which attribute is used to provide a unique identifier for an element to link it to a <label>?**
   - A) id
   - B) name
   - C) type
   - D) for

**7. If you want the browser to move the cursor automatically to a specific field when the page loads, which attribute do you use?**
   - A) active
   - B) selected
   - C) autofocus
   - D) required

**8. Which attribute provides a faint, temporary hint inside an input field describing the expected value?**
   - A) value
   - B) title
   - C) label
   - D) placeholder

**9. What happens to the form data when the method is set to "GET"?**
   - A) It is hidden in the body of the request.
   - B) It is appended to the URL in the address bar.
   - C) It is encrypted automatically.
   - D) It is not sent to the server.

**10. Which Boolean attribute prevents a form from being submitted if a specific field is empty?**
    - A) validated
    - B) mandatory
    - C) required
    - D) lock

**11. Which attribute is used to make a field uneditable, but still allows the value to be sent to the server?**
    - A) readonly
    - B) disabled
    - C) hidden
    - D) locked

**12. To allow a browser to suggest previously entered data for a form, which attribute should be set to "on"?**
    - A) remember
    - B) autocomplete
    - C) history
    - D) save

**13. In a group of radio buttons where the user should only pick ONE option, what attribute must they all share?**
    - A) id
    - B) value
    - C) name
    - D) type

**14. What is the primary purpose of the <fieldset> tag?**
    - A) To create a submit button.
    - B) To group related elements and draw a box around them.
    - C) To define the destination URL.
    - D) To create a drop-down menu.

**15. Which attribute of a <label> connects it to an input field's ID?**
    - A) for
    - B) link
    - C) target
    - D) to

**16. Which attribute determines the maximum number of characters a user can type into a text field?**
    - A) size
    - B) maxlength
    - C) length
    - D) limit

**17. What does the "value" attribute do for a text input field?**
    - A) It sets the default text that appears in the box.
    - B) It provides a hint to the user.
    - C) It names the field for the server.
    - D) It makes the field required.

**18. Which tag acts as the parent container for all form elements?**
    - A) <input>
    - B) <fieldset>
    - C) <form>
    - D) <label>

**19. What is the result of using 'method="POST"'?**
    - A) The data appears in the URL.
    - B) The data is sent in the HTTP request body.
    - C) The browser reloads the page without sending data.
    - D) The form is cleared instantly.

**20. Which attribute on the <form> tag specifies where to open the response (e.g., in a new tab)?**
    - A) action
    - B) method
    - C) path
    - D) target

---

### Part 2: Debugging Challenge (4 Points)

**21. The following code is intended to send the user's "username" to "login.php". However, when the user clicks submit, the server receives nothing. Find and fix the one error.**

```html
<form action="login.php" method="POST">
  <label for="user">Username:</label>
  <input type="text" id="user" placeholder="Enter name">
  <button type="submit">Login</button>
</form>