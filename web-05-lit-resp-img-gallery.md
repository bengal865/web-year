# Unit 05: Responsive Web Design

## Creating a Responsive Image Gallery Without Media Queries

Thanks to the CSS `repeat( )` function and keyword `auto-fit`, you can make your image gallery fully responsive with just a single line of code:

```css
.gallery-container {
  display: grid;
  /* The next line makes your image gallery fully responsive */
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}
```
---

## Breaking Down the Components of `repeat(auto-fit, minmax(250px, 1fr))`

### 1. The `repeat()` Function

**Purpose:** Efficiency. Instead of writing `1fr 1fr 1fr`, you tell the browser to repeat a pattern.

* **Essentialist logic:** Why define 3 columns or 4 columns manually when the browser can calculate the correct number of columns for you?

### 2. The `auto-fit` Keyword

**Purpose:** Flexibility. It tells the browser: "Fill the available space with as many columns as will fit based on the size I gave you."

* **The Difference:**
  * `auto-fill` creates empty ghost tracks even if there are no images.
  * `auto-fit` collapses empty tracks and stretches the existing items to fill the remaining space.
* **Essentialist logic:** `auto-fit` ensures there is no wasted white space on the right side of your gallery.

### 3. The `minmax()` Function

**Purpose:** The `minmax( )` function sets a floor and a ceiling for the item size.

* **`minmax(250px, 1fr)`**:
* **250px (The Floor):** An image can never be narrower than 250px. If the screen gets too small to hold 250px, the grid will wrap the item to a new row.
* **1fr (The Ceiling):** If there is extra space, the image can grow to fill 1 fraction of the available (or leftover) space.

* **Essentialist logic:** You define the the smallest acceptable width for the image, and let the browser automatically calculate the maximum width of each image.

---

## Responsive on Different Devices
Assuming you've set a minimum width of 250px for your image:
| Screen Size | Behavior |
| --- | --- |
| **Mobile (320px)** | The grid sees it can't fit two 250px items. It drops down to **1 column**. |
| **Tablet (600px)** | The grid fits two 250px items (500px total) and distributes the remaining 100px equally. **2 columns**. |
| **Desktop (1200px)** | The grid fits four 250px items (1000px total) and stretches them to fill the remaining space. **4 columns**. |

---

## Say No to Image Squishing

Make sure you also apply this CSS to your images so they don't break the grid container:

```css
img {
  width: 100%;
  height: auto;
  object-fit: cover; /* Ensures images don't look squished or distorted even if their aspect ratios -- original heights and widths -- vary */
}
```
