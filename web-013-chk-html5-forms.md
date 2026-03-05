## HTML5 Forms / Check
### Partners & Reading  

#### Names: _______________________________________

### Directions

- Read the info about HTML5 [input fields](https://www.w3schools.com/html/html_form_input_types.asp) first
- Review the questions below with your partner
- Answer the questions about the reading assignment
- Be prepared to share your answers with the class

---

1. In plain English, explain what a **form handler** is.  

2. If you don't use the `value` attribute with a submit button, what will be the default text on the button?  

```html
<form action="/action_page.php">
  <label for="fname">First Name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last Name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form>
```  

3. What patterns do you notice in the code below?  

```html
<form action="/action_page.php">
  <label for="fname">First Name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last Name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form>
```  

4. How does a radio button work differently than a checkbox?  

5. What is the `step` attribute used for in the code below?  
```html
<form>
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
</form>
```  

6. You have a text input field and radio buttons on your web form.  What are the advantages and disadvantages of each type of input field?

```html
<form action="/action_page.php">
  <label for="fname">First Name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last Name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>

  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>  
```  

7. What are some problems you could have when using a web form to collect data from users?  (List 2 - 3 possible problems)

Problem 1: ___________________________________________  
Problem 2: ___________________________________________  
Problem 3: ___________________________________________


