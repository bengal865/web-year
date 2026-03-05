### Summary of Form Field Attributes / Dino's Pizza Order Form

* **First Name & Last Name**
    * `type="text"`: Defines a single-line text field.
    * `id`: Unique identifier used to link the input to its `<label>`.
    * `name`: The key used to identify the data when sent to the server.
    * `placeholder`: Provides a short hint of the expected value.
    * `required`: Forces the user to enter text before the form can be submitted.

* **Email**
    * `type="email"`: Automatically validates that the entry follows a proper email format (e.g., name@domain.com).
    * `autocomplete="email"`: Allows browsers to suggest the user's saved email addresses.
    * `id`, `name`, `placeholder`, `required`: (Standard attributes).

* **Phone**
    * `type="tel"`: Optimizes the input for telephone numbers, often triggering a dial-pad on mobile.
    * `pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}"`: Uses a regular expression to enforce the 123-456-7890 format.
    * `autocomplete="tel"`: Enables browser autofill for phone numbers.
    * `id`, `name`, `placeholder`, `required`: (Standard attributes).

* **Toppings (Checkboxes)**
    * `type="checkbox"`: Allows the user to select zero, one, or multiple options from the list.
    * `value`: The specific data (e.g., "pepperoni") sent to the server if the box is checked.
    * `id`, `name`: (Standard attributes).

* **Size, Crust, & Credit Card Issuer (Radio Buttons)**
    * `type="radio"`: Groups options so that only one selection can be made at a time.
    * `checked`: Pre-selects a default option (Small, Thin Crust, and VISA) when the page loads.
    * `required`: Ensures that at least one radio button in the group is selected.
    * `id`, `name`, `value`: (Standard attributes).

* **Card Number**
    * `type="text"`: Standard text input used here to allow for pattern flexibility.
    * `inputmode="numeric"`: Specifically requests a numeric keypad on mobile devices for ease of entry.
    * `autocomplete="cc-number"`: Enables secure browser autofill for credit card numbers.
    * `maxlength="19"`: Prevents the user from entering more than 19 characters (accounting for spaces).
    * `pattern="[0-9\s]{13,19}"`: Restricts input to numbers and spaces, between 13 and 19 characters long.
    * `required`: (Standard attribute).

* **Expiration Month**
    * `type="text"`: Standard text input.
    * `inputmode="numeric"`: Triggers a numeric keypad on mobile devices.
    * `autocomplete="cc-exp-month"`: Allows the browser to autofill just the expiration month.
    * `pattern="(0[1-9]|1[0-2])"`: Enforces a two-digit month format (01 through 12).
    * `maxlength="2"`: Limits entry to exactly two digits.
    * `required`: (Standard attribute).

* **Expiration Year**
    * `type="text"`: Standard text input.
    * `inputmode="numeric"`: Triggers a numeric keypad.
    * `autocomplete="cc-exp-year"`: Allows the browser to autofill just the expiration year.
    * `pattern="[0-9]{4}"`: Enforces a four-digit year format (e.g., 2026).
    * `maxlength="4"`: Limits entry to exactly four digits.
    * `required`: (Standard attribute).

* **Card Security Code (CVV)**
    * `type="text"`: Standard text input.
    * `inputmode="numeric"`: Triggers a numeric keypad.
    * `pattern="[0-9]{3,4}"`: Validates that the entry is exactly 3 or 4 digits.
    * `autocomplete="cc-csc"`: Enables browser autofill for security codes.
    * `required`: (Standard attribute).

* **Submit Button**
    * `type="submit"`: A specialized button that automatically gathers form data and sends it to the `action` URL.
    * `value="Submit Order"`: Sets the text displayed on the button.
