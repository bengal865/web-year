
---

### Part 2: Debugging Challenge (4 Points)

**21. The following code is intended to send the user's "username" to "login.php". However, when the user clicks submit, the server receives nothing. Find and fix the one error.**

```html
<form action="login.php" method="POST">
  <label for="user">Username:</label>
  <input type="text" id="user" placeholder="Enter name">
  <button type="submit">Login</button>
</form>

```

**What is the error?** ___________________________________________________________

---

# Answer Key and Explanations

1. **C) action** (Defines the destination address).
2. **B) <optgroup>** (Used to categorize options in a select menu).
3. **D) GET** (Default browser behavior).
4. **B) name** (The server uses this as the 'key' to find the data).
5. **B) POST** (Keeps sensitive data out of the URL).
6. **A) id** (Labels use the 'for' attribute to find the input's 'id').
7. **C) autofocus** (Focuses the element on page load).
8. **D) placeholder** (The faint hint text).
9. **B) It is appended to the URL** (Visible in the address bar).
10. **C) required** (Enforces browser-level validation).
11. **A) readonly** (Disabled fields do not send data; readonly fields do).
12. **B) autocomplete** (Controls the browser's memory of past entries).
13. **C) name** (Sharing a name creates a mutual exclusion group).
14. **B) Grouping elements** (Visually and logically organizes form sections).
15. **A) for** (The label's 'for' attribute must match the input's 'id').
16. **B) maxlength** (Limits character count).
17. **A) Sets default text** (Populates the field with an actual value).
18. **C) <form>** (The main wrapper).
19. **B) Sent in request body** (Standard for secure or large data).
20. **D) target** (Use `_blank` for a new tab).

**Debugging Answer:**
The `<input>` tag is missing the **name** attribute.

* **Corrected line:** `<input type="text" id="user" name="username" placeholder="Enter name">`
* **Explanation:** Without a `name` attribute, the browser does not know what to call the data, so it doesn't send it to the server.

