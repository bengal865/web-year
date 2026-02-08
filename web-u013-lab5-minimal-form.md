# 013 HTML Forms
### Styling Your Shipping Form

## 1. General Web Page Styling

Set the foundation for the page typography and layout.

* **Font Family:** Set the `body` to a sans-serif stack (e.g., `-apple-system`, `Arial`, or `sans-serif`).
* **Page Layout:** Set `max-width` to `500px`, `margin` to `auto`, and add `padding` to center the form and give it breathing room.
* **Background:** Apply a light gray (`#f9f9f9`) to the `body` to make the white form stand out.

## 2. Form Container and Typography

Style the "box" that holds the inputs.

* **Container Box:** Set the `form` background to white, add a `25px` padding, and a subtle `box-shadow` for depth.
* **Headings:** Add a `border-bottom` to the `h1` to separate the form's title from its fields.
* **Labels:** Set `label` to `display: block` so they sit above the inputs, and use `font-weight: 600` for readability.

## 3. Input and Select Elements

Make the interactive fields easy to use and consistent.

* **Width & Sizing:** Set `input[type="text"]`, `input[type="email"]`, and `select` to `width: 100%`.
* **Box Model:** Use `box-sizing: border-box` to ensure padding doesn't push the inputs outside the container.
* **Spacing:** Add `8px` of internal padding and a small `margin-bottom` to separate fields.
* **Focus State:** Add an `input:focus` rule to change the `border-color` to blue (`#007bff`) when a user clicks inside.

## 4. Fieldsets and Layout Groups

Organize the radio buttons and checkboxes.

* **Fieldsets:** Set a light `1px` border and `15px` padding to group the payment methods.
* **Inline Labels:** For radio buttons and checkboxes, override the block display by setting their specific labels to `display: inline`.
* **Alignment:** Use `display: flex` and `align-items: flex-start` on a wrapper class for the Terms and Conditions to keep the text aligned with the checkbox.

## 5. Submit Button Styling

Create a clear Call to Action (CTA).

* **Colors:** Set the background to a dark color (`#333`) and text to white.
* **Padding:** Use `10px 20px` to make the button a large, clickable target.
* **Hover Effect:** Add a `transition` and change the `background-color` to a lighter gray on hover to provide visual feedback.
* **Width:** Set the button to `width: 100%` to match the inputs above it.

