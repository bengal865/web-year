This script is designed for a **45–60 minute live-coding session**. It assumes you are starting with a blank slate (or the "Broken HTML" from earlier) and moving toward the "Pure Grid" final version.

---

## Part 1: The "Why" and the Setup (5 mins)

**Teacher:** "Alright class, we’ve learned how to make beautiful layouts with CSS Grid. But a website isn't a one-way street; we need to talk back to it. That’s what **Forms** are for. Today, we’re building a registration page for *Apex Nebula*. We’re going to use Grid twice: once to center the whole page, and once to 'draw' our form layout using **Template Areas**."

**Action:** Open a blank `index.html` and `style.css`. Create the basic HTML boilerplate.

---

## Part 2: Building the Accessible Skeleton (10 mins)

**Teacher:** "First, the HTML. We aren't just throwing inputs on a page. We need **Labels**. If a screen reader hits your page and there’s no label, the user has no idea what to type. Also, look at this..."

**Action:** Type the username field.

```html
<label for="username">Username</label>
<input type="text" id="username" name="username">

```

**Teacher:** "Notice the `for` and the `id`. They are twins. If they match, you can click the word 'Username' and the box highlights. That’s a huge UX win for mobile users with big thumbs."

**Action:** Add the Email and Textarea fields, explaining the `type="email"` benefit (automatic validation).

---

## Part 3: The Macro-Layout (The Body Grid) (10 mins)

**Teacher:** "Now to the CSS. We want our form dead-center on the screen. Usually, we'd use Flexbox, but we’re Grid masters now. Let's make the entire `<body>` a Grid."

**Action:** Add this to `style.css`:

```css
body {
    display: grid;
    grid-template-rows: 1fr auto; 
    min-height: 100vh;
}

```

**Teacher:** "Look at `grid-template-rows: 1fr auto;`. The `1fr` tells the main section to gobble up all the empty space, pushing our footer to the very bottom. It’s the easiest 'sticky footer' you’ll ever make."

---

## Part 4: The "Tetris" Method (Template Areas) (15 mins)

**Teacher:** "Now for the magic. We want the labels on the left and inputs on the right. Instead of calculating percentages, we are going to **map** it out."

**Action:** Wrap the labels and inputs in a `.field-container` and add this CSS:

```css
.field-container {
    display: grid;
    grid-template-columns: 150px 1fr;
    grid-template-areas: 
        "label-user  input-user"
        "label-mail  input-mail"
        "label-bio   input-bio"
        ".           button";
    gap: 20px;
}

```

**Teacher:** "Look at the `grid-template-areas`. I am literally drawing the layout. That `.` in the last row? That’s an empty space. It keeps our button under the inputs rather than stretching across the whole screen. Now, we just tell the elements where they belong."

**Action:** Assign the `grid-area` to each element (e.g., `label { grid-area: label-user; }`).

---

## Part 5: The "Mobile Snap" (10 mins)

**Teacher:** "Final step. This looks great on a laptop, but it’ll look squashed on a phone. Let’s redefine our map for mobile."

**Action:** Add the Media Query.

```css
@media (max-width: 600px) {
    .field-container {
        grid-template-columns: 1fr;
        grid-template-areas: 
            "label-user"
            "input-user"
            "label-mail"
            "input-mail";
    }
}

```

**Teacher:** "By changing the map to a single column, we just 'snapped' our form into a mobile-friendly stack. No floats, no hacks—just a new list of names."

---

## Part 6: Wrap Up & Challenge

**Teacher:** "You’ve got the structure. Now, spend the rest of the period styling your inputs. Use the `:focus` pseudo-class to make them glow when clicked. Make this look like a premium gaming site!"

