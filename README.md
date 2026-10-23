# 🚀 Frontend Interview Mastery: HTML, CSS & Accessibility

Here is the fully formatted, professionally styled Markdown version of your document. All content has been preserved, and code snippets, tags, and properties have been properly highlighted for maximum readability.

---

### 📌 Q1 — What is Semantic HTML?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Semantic HTML means using HTML elements according to their meaning and purpose, such as `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, and `<button>`, instead of using `<div>` for everything.
It improves accessibility, SEO, and code readability.

**🔗 Follow-up:**
_What's the difference between `<div>` and `<section>`?_

---

### 📌 Q2 — What is the difference between `<div>` and `<span>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<div>` is a generic block-level container, while `<span>` is a generic inline-level container.
For example, I can use `<div>` to group sections of a layout and `<span>` to style or group a small part of text.

**🔗 Follow-up:**
_Can CSS change their default display behavior?_
**↳ Answer:**
Yes. For example, I can make a `<div>` inline using `display: inline`, or make a `<span>` block-level using `display: block`.

---

### 📌 Q3 — What is the DOM?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
The DOM, or Document Object Model, is a tree-like representation of the HTML document created by the browser. JavaScript can use the DOM to read, modify, add, or remove elements and attributes.

**🔗 Follow-up:**
_Does the DOM equal the HTML source code?_
**↳ Answer:**
Not exactly. The browser parses the HTML and creates the DOM. The DOM can then be modified by JavaScript, so it can differ from the original HTML source.

---

### 📌 Q4 — What is the difference between `id` and `class`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
An `id` is intended to uniquely identify an element within a document, while a `class` can be shared by multiple elements.
For styling reusable elements, I normally use classes.

**🔗 Follow-up:**
_Can multiple elements have the same ID?_
**↳ Answer:**
Technically browsers may still render the page, but IDs are intended to be unique, so using the same ID multiple times is invalid HTML and can cause problems with JavaScript, CSS, and accessibility.

---

### 📌 Q5 — What is the difference between `block`, `inline`, and `inline-block`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

1. **`block`**: normally starts on a new line and takes the available width.
2. **`inline`**: stays within the text flow and generally doesn't respect width/height in the same way.
3. **`inline-block`**: stays inline but allows width and height to be applied.

**🔗 Follow-up:**
_Give examples._
**↳ Answer:** `<div>` is normally block, `<span>` is normally inline, and a button can behave like an inline-block element depending on browser defaults/styles.

---

### 📌 Q6 — What is the CSS Box Model?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Every element is represented as a box consisting of:
`content` → `padding` → `border` → `margin`
The content contains the actual content, padding is space inside the border, border surrounds the element, and margin creates space outside the element.

**🔗 Follow-up:**
_What does `box-sizing: border-box` do?_
**↳ Answer:**
It makes the declared width and height include the element's content, padding, and border.

---

### 📌 Q7 — What is CSS specificity?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Specificity is the mechanism browsers use to determine which CSS rule has higher priority when multiple rules target the same element.
Generally, inline styles have higher specificity than IDs, IDs higher than classes/attributes/pseudo-classes, and those higher than element selectors.

**🔗 Follow-up:**
_What is more specific: `.button` or `#button`?_
**↳ Answer:** `#button`.

---

### 📌 Q8 — What is Flexbox?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Flexbox is a one-dimensional CSS layout system designed to arrange elements along a row or column.
It provides properties such as `display: flex`, `justify-content`, `align-items`, `flex-direction`, `gap`, and `flex-wrap`.

**🔗 Follow-up:**
_What is the difference between `justify-content` and `align-items`?_
**↳ Answer:**
Their effect depends on the flex direction. Generally, `justify-content` controls distribution along the main axis, while `align-items` controls alignment along the cross axis.

---

### 📌 Q9 — What is CSS Grid?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
CSS Grid is a two-dimensional layout system that works with rows and columns. It's useful for complex page layouts and structured grids.

**🔗 Follow-up:**
_Flexbox or Grid for a product grid?_
**↳ Answer:**
Either can work, but Grid is often a natural choice when I need explicit row/column control. Flexbox is often better for one-dimensional layouts such as navigation bars or aligning items in a row.

---

### 📌 Q10 — What is Responsive Design?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Responsive design means building interfaces that adapt to different screen sizes and devices.
I can achieve this using flexible layouts, CSS Grid/Flexbox, relative units, media queries, responsive images, and appropriate breakpoints.

**🔗 Follow-up:**
_How would you make an Angular dashboard responsive?_
**↳ Answer:**
I'd first build a flexible layout using Grid/Flexbox, then introduce breakpoints for major layout changes, and use responsive components from the UI library when appropriate.

---

### 📌 Q11 — What is the difference between `<section>` and `<article>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`<section>` represents a thematic grouping of content within a page, while `<article>` represents a self-contained piece of content that could potentially stand on its own or be distributed independently.
For example, a blog page could have multiple `<article>` elements, while `<section>` could group related content such as "Latest Posts" or "Contact Information."

**🔗 Follow-up:**
_Can an `<article>` contain a `<section>`?_
**↳ Answer:**
Yes. An article can contain sections when the article itself has multiple thematic parts.

---

### 📌 Q12 — What is the difference between `<strong>` and `<b>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<strong>` gives semantic importance to its content, while `<b>` mainly indicates that the text should be stylistically distinguished without adding the same semantic importance.
For example:

```html
<strong>Warning:</strong> Your account will expire.
```

Here, "Warning" has semantic importance.

**🔗 Follow-up:**
_Does `<strong>` necessarily make text bold?_
**↳ Answer:**
Browsers usually render it as bold by default, but its important part is the semantic meaning, not the visual appearance. CSS controls the actual presentation.

---

### 📌 Q13 — What is the difference between `<em>` and `<i>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<em>` represents emphasized content semantically, while `<i>` represents text that is stylistically offset from the surrounding content without necessarily indicating emphasis.
For example, `<em>` can indicate that a word should be emphasized when the sentence is read.

**🔗 Follow-up:**
_Are `<em>` and `<i>` always displayed differently?_
**↳ Answer:**
By default, browsers commonly render both as italic, but their semantic meanings are different.

---

### 📌 Q14 — Why should we use `<button>` instead of a clickable `<div>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
A `<button>` is designed specifically for user actions. It provides built-in keyboard accessibility, focus behavior, semantics for assistive technologies, and standard browser behavior.
A `<div>` is only a generic container, so if I make it clickable, I'd have to manually reproduce behaviors such as keyboard interaction and accessibility semantics.

**🔗 Follow-up:**
_What if the clickable element navigates to another page?_
**↳ Answer:**
I would generally use an `<a>` element because navigation is the semantic purpose of a link.

---

### 📌 Q15 — What is the difference between `<a>` and `<button>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
An `<a>` is primarily used for navigation to another URL or resource, while a `<button>` is used to perform an action.
For example:

```html
<a href="/profile">Profile</a>
<!-- Navigation -->
<button type="button">Open Modal</button>
<!-- Action -->
```

**🔗 Follow-up:**
_What would you use for a "Delete Account" action?_
**↳ Answer:**
A `<button>`, because deleting is an action, not navigation.

---

### 📌 Q16 — What is the purpose of the `alt` attribute in an `<img>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
The `alt` attribute provides alternative text describing the image. It's useful for screen readers and is also displayed or exposed when the image cannot be loaded.
For meaningful images, the `alt` should describe their purpose or content.
For purely decorative images, the `alt` can be empty:

```html
<img src="decoration.png" alt="" />
```

**🔗 Follow-up:**
_Should we put "image of..." in every `alt`?_
**↳ Answer:**
Not necessarily. The screen reader already knows it's an image, so the alt text should focus on the useful information rather than unnecessarily saying "image of."

---

### 📌 Q17 — What is the difference between `id`, `class`, and `name` attributes?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

1. **`id`** identifies an element uniquely within the document.
2. **`class`** is used to group elements for styling or JavaScript behavior.
3. **`name`** identifies a form control when its value is submitted as part of form data.

For example:

```html
<input id="email" name="email" class="form-control" type="email" />
```

Here, `id` can be associated with a `<label>`, `class` can be used for styling, and `name` is important when submitting form data.

**🔗 Follow-up:**
_Why do we usually connect `<label>` to the input using `for` and `id`?_
**↳ Answer:**
It associates the label with the input, improving accessibility and allowing users to focus the input by clicking the label.

---

### 📌 Q18 — What is the purpose of the `<label>` element?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<label>` provides a textual description for a form control and improves accessibility.
It can be associated with an input using `for`:

```html
<label for="email">Email</label> <input id="email" type="email" />
```

Clicking the label will also focus or activate the associated control.

**🔗 Follow-up:**
_Can we wrap the input inside the label?_
**↳ Answer:**
Yes.

```html
<label>
  Email
  <input type="email" />
</label>
```

This creates an implicit association between the label and the input.

---

### 📌 Q19 — What is the difference between `GET` and `POST` when submitting an HTML form?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
With a traditional HTML form:

1. **`GET`** sends form data as part of the URL query string.
2. **`POST`** sends the data in the request body.

`GET` is commonly used for retrieving/searching data, while `POST` is commonly used for submitting data that causes a server-side operation.
For example:

```html
<form method="GET">
  <!-- Search filters -->
  <form method="POST"><!-- Registration data --></form>
</form>
```

**🔗 Follow-up:**
_Is POST automatically secure?_
**↳ Answer:**
No. POST does not provide encryption by itself. HTTPS is what encrypts the communication between the client and server.

---

### 📌 Q20 — What is the difference between `disabled` and `readonly` on an input?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`disabled` means the control cannot be interacted with and is generally excluded from form submission.
`readonly` means the user cannot modify the value, but the control can still generally be focused and its value can participate in form submission.

Example:

```html
<input value="Youssef" readonly />
<!-- Focusable, not editable -->
<input value="Youssef" disabled />
<!-- Disabled entirely -->
```

**🔗 Follow-up:**
_Can JavaScript change a `readonly` input?_
**↳ Answer:**
Yes. `readonly` prevents the user from editing it through the normal UI, but JavaScript can still modify its value.

---

### 📌 Q21 — What is the difference between `<head>` and `<body>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
The `<head>` contains metadata and resources about the document, such as the `<title>`, meta tags, stylesheets, and scripts that need to be loaded.
The `<body>` contains the actual content that is rendered and displayed to the user, such as headings, paragraphs, images, forms, and buttons.

**🔗 Follow-up:**
_Is everything inside `<head>` invisible to the user?_
**↳ Answer:**
Most of the content isn't directly displayed, but some elements can affect browser behavior or load resources. For example, `<title>` appears in the browser tab.

---

### 📌 Q22 — What is the purpose of the `<meta viewport>` tag?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
The viewport meta tag tells the browser how to control the page's dimensions and scaling on mobile devices.
The common version is:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

`width=device-width` makes the viewport width match the device's CSS width, while `initial-scale=1.0` sets the initial zoom level.

**🔗 Follow-up:**
_What can happen if we don't include it on a mobile page?_
**↳ Answer:**
The browser may use a wider virtual viewport, causing the page to appear zoomed out and making responsive layouts behave incorrectly.

---

### 📌 Q23 — What is the purpose of the `DOCTYPE` declaration?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<!DOCTYPE html>` tells the browser that the document should be interpreted using the modern HTML standard and helps the browser use standards mode instead of quirks mode.

**🔗 Follow-up:**
_Is `DOCTYPE` an HTML element?_
**↳ Answer:**
No. It's a document type declaration, not an HTML element.

---

### 📌 Q24 — What is the difference between `localStorage`, `sessionStorage`, and cookies?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
All three can store client-side data, but they behave differently.

1. **`localStorage`** persists until it's explicitly cleared.
2. **`sessionStorage`** usually persists only for the lifetime of the browser tab/session.
3. **Cookies** are small pieces of data associated with HTTP requests and can be configured with attributes such as `HttpOnly`, `Secure`, and `SameSite`.

Cookies can automatically be sent to the server, while `localStorage` and `sessionStorage` are not automatically included in HTTP requests.

**🔗 Follow-up:**
_Which is safer for storing an authentication token?_
**↳ Answer:**
It depends on the authentication architecture and threat model. For tokens that should be protected from JavaScript access, an `HttpOnly`, `Secure`, appropriately configured cookie can reduce XSS exposure compared with storing the token in `localStorage`. However, cookie-based authentication introduces CSRF considerations that must also be handled.

---

### 📌 Q25 — What is the difference between `async` and `defer` for scripts?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Both `async` and `defer` allow scripts to download without blocking HTML parsing.

- With **`async`**, the script executes as soon as it finishes downloading, so execution order between multiple `async` scripts isn't guaranteed.
- With **`defer`**, scripts execute after HTML parsing is complete, and deferred scripts maintain their document order.

**🔗 Follow-up:**
_Which would you prefer when one script depends on another?_
**↳ Answer:** `defer` is generally more appropriate when script execution order matters because deferred scripts execute in document order.

---

### 📌 Q26 — What is accessibility in HTML?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Web accessibility means making websites usable by people with different abilities, including users who rely on assistive technologies such as screen readers or keyboard navigation.
In HTML, I can improve accessibility by using semantic elements, proper labels for forms, meaningful `alt` text, correct heading structure, keyboard-accessible controls, and appropriate ARIA attributes when necessary.

**🔗 Follow-up:**
_Should we use ARIA everywhere?_
**↳ Answer:**
No. Native semantic HTML should be preferred whenever possible. ARIA should be used when native HTML semantics aren't sufficient for a specific custom component or interaction.

---

### 📌 Q27 — What is ARIA?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
ARIA stands for Accessible Rich Internet Applications. It provides attributes that communicate roles, states, and properties of UI elements to assistive technologies.
For example:

```html
<button aria-label="Close dialog">×</button>
```

The `aria-label` gives the button an accessible name.

**🔗 Follow-up:**
_Give me examples of ARIA attributes._
**↳ Answer:**
Examples include `aria-label`, `aria-labelledby`, `aria-describedby`, `aria-expanded`, `aria-hidden`, and `aria-selected`.

---

### 📌 Q28 — What is the difference between `aria-label` and `aria-labelledby`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**  
`aria-label` directly provides an accessible name as a string.
`aria-labelledby` references another element whose text provides the accessible name.
For example:

```html
<h2 id="dialog-title">Delete Account</h2>
<div role="dialog" aria-labelledby="dialog-title">...</div>
```

The dialog gets its accessible name from the `<h2>`.

**🔗 Follow-up:**
_When would you prefer `aria-labelledby`?_
**↳ Answer:**
When there is already visible text that appropriately names the element. Referencing that text avoids duplicating the same label.

---

### 📌 Q29 — What is the difference between `autocomplete`, `placeholder`, and `value`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

1. **`placeholder`** provides a temporary hint about what the user should enter.
2. **`value`** represents the actual current value of the input.
3. **`autocomplete`** gives the browser information about what kind of information the field expects so it can provide autofill suggestions.

For example:

```html
<input
  type="email"
  name="email"
  autocomplete="email"
  placeholder="Enter your email"
/>
```

**🔗 Follow-up:**
_Should placeholder replace a label?_
**↳ Answer:**
No. A placeholder is not a proper replacement for a label because it disappears when the user starts typing and can create accessibility and usability issues.

---

### 📌 Q30 — What is the difference between `<ul>`, `<ol>`, and `<dl>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

1. **`<ul>`** represents an unordered list where item order isn't important.
2. **`<ol>`** represents an ordered list where sequence matters.
3. **`<dl>`** represents a description list consisting of terms and their descriptions.

Example:

```html
<ul>
  <li>Angular</li>
  <li>Spring Boot</li>
</ul>

<!-- For steps -->
<ol>
  <li>Login</li>
  <li>Select a product</li>
  <li>Checkout</li>
</ol>

<!-- And a term/description -->
<dl>
  <dt>Angular</dt>
  <dd>A frontend web framework.</dd>
</dl>
```

**🔗 Follow-up:**
_Can CSS remove the bullets from a `<ul>`?_
**↳ Answer:**
Yes. For example, `list-style: none` can remove the default markers. But removing the visual bullets doesn't change the semantic meaning of the element.

---

### 📌 Q31 — What is the difference between an HTML element and an HTML attribute?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
An HTML element is a complete building block of the document, such as `<p>`, `<div>`, or `<input>`.
An attribute provides additional information or configuration about an element.
For example:

```html
<input type="email" id="email" required />
```

Here, `<input>` is the element, while `type`, `id`, and `required` are attributes.

**🔗 Follow-up:**
_Are all HTML elements allowed to have the same attributes?_
**↳ Answer:**
No. Some attributes are global and can be used on many elements, such as `id`, `class`, and `title`, while others are specific to particular elements, such as `src` for images.

---

### 📌 Q32 — What are global HTML attributes?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Global attributes are attributes that can generally be used on most HTML elements.
Examples include:

1. `id`
2. `class`
3. `title`
4. `style`
5. `hidden`
6. `tabindex`
7. `data-*`
8. `aria-*`

For example:

```html
<div id="profile" class="card" title="User profile"></div>
```

**🔗 Follow-up:**
_What are `data-_` attributes?\*
**↳ Answer:**
They allow developers to store custom data associated with an HTML element.
For example:

```html
<button data-user-id="123">Delete</button>
```

JavaScript can access it through the element's `dataset`.

---

### 📌 Q33 — What is the difference between `data-*` attributes and normal attributes?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`data-*` attributes are specifically intended for storing custom data on HTML elements without creating non-standard HTML attributes.
For example:

```html
<div data-product-id="25" data-category="plants"></div>
```

In JavaScript:

```javascript
element.dataset.productId; // would access the data-product-id value.
```

**🔗 Follow-up:**
_Should sensitive information be stored in `data-_` attributes?\*
**↳ Answer:**
No. Anything in the HTML is accessible to the client and should be treated as public. Sensitive information such as passwords or secret tokens should never be exposed there.

---

### 📌 Q34 — What is the difference between `absolute`, `relative`, `fixed`, and `sticky` positioning?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

1. **`relative`**: the element remains in the normal document flow but can be visually offset; it can also establish a containing block for positioned descendants.
2. **`absolute`**: the element is removed from normal flow and is positioned relative to its containing block.
3. **`fixed`**: the element is removed from normal flow and is positioned relative to the viewport in typical cases.
4. **`sticky`**: the element behaves like relatively positioned content until a threshold is reached, then sticks within its scrolling container.

**🔗 Follow-up:**
_Relative to what is an absolutely positioned element positioned?_
**↳ Answer:**
Usually to its nearest ancestor that establishes a positioning context, commonly an ancestor with `position: relative`, `absolute`, `fixed`, or `sticky`. If there isn't one, the containing block can be the initial containing block.

---

### 📌 Q35 — What is the difference between `<script>`, `<script async>`, and `<script defer>`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
A normal `<script>` can block HTML parsing while the browser fetches and executes the script.

- With **`async`**, the script downloads in parallel with HTML parsing and executes as soon as it's available. Therefore, execution order between `async` scripts isn't guaranteed.
- With **`defer`**, the script also downloads in parallel, but execution happens after HTML parsing is complete, and deferred scripts maintain their document order.

**🔗 Follow-up:**
_Which one is usually appropriate for scripts that depend on the DOM?_
**↳ Answer:** `defer` is usually a good choice because the script executes after the HTML has been parsed.

---

### 📌 Q36 — What is the difference between `<link>` and `<a>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`<a>` creates a hyperlink that users can interact with to navigate to another resource.
`<link>` defines a relationship between the current document and an external resource. It's commonly used in the `<head>` to load stylesheets.

For example:

```html
<link rel="stylesheet" href="styles.css" />
<!-- Metadata/resource relationship -->
<a href="/about">About Us</a>
<!-- Interactive hyperlink -->
```

**🔗 Follow-up:**
_Can `<link>` be placed inside `<body>`?_
**↳ Answer:**
Some link relationships have specific placement rules, but stylesheet links are conventionally placed in the `<head>`. The key distinction is that `<link>` is metadata/resource relationship, while `<a>` is an interactive hyperlink.

---

### 📌 Q37 — What is the difference between `required`, `disabled`, and `readonly`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

1. **`required`** means the user must provide a value for the field for form validation to succeed.
2. **`disabled`** means the control is disabled and cannot normally be interacted with; disabled form controls are generally excluded from native form submission.
3. **`readonly`** means the user cannot modify the value, but the control remains generally usable and its value can be submitted.

Example:

```html
<input name="email" required />
<input name="userId" value="123" readonly />
<input name="status" value="active" disabled />
```

**🔗 Follow-up:**
_If I have a disabled input, can JavaScript read its value?_
**↳ Answer:**
Yes. Disabling the input doesn't erase its value. JavaScript can still access the element and its value.

---

### 📌 Q38 — What is the difference between `hidden` and `display: none`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
The `hidden` HTML attribute indicates that an element is not currently relevant to the user and the browser normally doesn't render it.
`display: none` is a CSS rule that removes the element from the rendered layout.

For example:

```html
<div hidden>Hidden content</div>
```

and:

```css
.hidden {
  display: none;
}
```

Both normally result in the element not being visually rendered, but they communicate different intent: `hidden` is an HTML semantic state, while `display: none` is presentation.

**🔗 Follow-up:**
_Does `display: none` take space in the layout?_
**↳ Answer:**
No. The element doesn't occupy layout space.

---

### 📌 Q39 — What is the difference between `visibility: hidden` and `display: none`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`display: none` removes the element from the layout, so it doesn't occupy space.
`visibility: hidden` makes the element invisible, but it normally remains in the layout and keeps its space.

**🔗 Follow-up:**
_What about `opacity: 0`?_
**↳ Answer:** `opacity: 0` makes the element fully transparent, but the element can still occupy layout space and can potentially remain interactive depending on the situation.

---

### 📌 Q40 — What is the difference between `<iframe>` and `<embed>`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`<iframe>` embeds another HTML browsing context inside the current page. It's commonly used for embedding external pages, maps, videos, or other web content.
`<embed>` is a more general element for embedding external content, historically including plugins and certain document/media formats.
For modern web applications, `<iframe>` is much more commonly encountered for embedding another web page or external browsing context.

**🔗 Follow-up:**
_Can an iframe communicate with its parent page?_
**↳ Answer:**
Yes. JavaScript can communicate between windows/frames using mechanisms such as `postMessage`, especially when dealing with cross-origin contexts.

---

### 📌 Q41 — What is the difference between `<header>`, `<nav>`, `<main>`, `<aside>`, and `<footer>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
They are semantic elements that describe different structural parts of a page:

1. **`<header>`** represents introductory content for a page or section.
2. **`<nav>`** contains major navigation links.
3. **`<main>`** contains the primary content of the document.
4. **`<aside>`** contains related or supplementary content.
5. **`<footer>`** contains footer information for a page or section.

**🔗 Follow-up:**
_Can a page have multiple `<header>` or `<footer>` elements?_
**↳ Answer:**
Yes. They can be used for the document itself or for individual sections/articles. However, a document should generally have one primary `<main>` element.

---

### 📌 Q42 — Can an HTML page have multiple `<main>` elements?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
A document should have only one visible `<main>` element representing the dominant content of the document.
If I have multiple sections or views, I wouldn't normally put multiple visible `<main>` elements on the same page.

**🔗 Follow-up:**
_Can the `<main>` element be nested inside `<article>` or `<section>`?_
**↳ Answer:**
Normally, `<main>` should represent the main content of the document and shouldn't be nested inside elements such as `article`, `aside`, `footer`, `header`, or `nav`.

---

### 📌 Q43 — What is the difference between `<br>` and `<p>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<p>` represents a paragraph, while `<br>` represents a line break within the current text flow.

A `<br>` can be used when an actual line break is part of the content:

```html
Address Line 1<br />
Address Line 2
```

**🔗 Follow-up:**
_Should I use multiple `<br>` elements to create vertical spacing?_
**↳ Answer:**
No. Layout and spacing should generally be handled with CSS such as `margin` and `padding`.

---

### 📌 Q44 — What is the difference between `<p>` and `<div>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<p>` represents a paragraph of text and has semantic meaning.
`<div>` is a generic container with no specific semantic meaning.
So if I'm displaying a paragraph, I should use `<p>` rather than `<div>`.

**🔗 Follow-up:**
_Can a `<p>` contain a `<div>`?_
**↳ Answer:**
No. A `<div>` is not valid as a descendant of a paragraph because `<p>` has specific content-model rules. The browser may automatically close the paragraph before the `<div>`.

---

### 📌 Q45 — What is the difference between `<textarea>` and `<input type="text">`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<input type="text">` is designed for a single-line text value, while `<textarea>` is designed for multi-line text.
For example, a username would typically use an input, while a message or description would typically use a `<textarea>`.

**🔗 Follow-up:**
_Can `<textarea>` have a `value` attribute?_
**↳ Answer:**
The initial value of a `<textarea>` is normally provided as its text content:

```html
<textarea>Hello</textarea>
```

rather than using a `value` attribute like an input.

---

### 📌 Q46 — What is the purpose of the `name` attribute in form controls?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
The `name` attribute identifies a form control when the browser constructs the form data for submission.
For example:

```html
<form>
  <input name="username" />
  <input name="email" />
</form>
```

The submitted data can contain key-value pairs such as: `username=Youssef`, `email=test@example.com`.

**🔗 Follow-up:**
_Does an input need `name` to work with JavaScript?_
**↳ Answer:**
No. JavaScript can access the input using its ID, class, DOM reference, or other selectors. But `name` has an important role in native HTML form submission.

---

### 📌 Q47 — Why do radio buttons usually share the same `name`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Radio buttons with the same `name` belong to the same group, so the user can normally select only one option from that group.
For example:

```html
<input type="radio" name="gender" value="male" />
<input type="radio" name="gender" value="female" />
```

Because both have `name="gender"`, they behave as one radio group.

**🔗 Follow-up:**
_What happens if they have different names?_
**↳ Answer:**
They are treated as separate groups, so the user can select one option from each group.

---

### 📌 Q48 — What is the difference between `<select>`, `<option>`, and `<optgroup>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**

1. **`<select>`** represents the dropdown control.
2. **`<option>`** represents an individual selectable item.
3. **`<optgroup>`** groups related options inside a select.

Example:

```html
<select name="country">
  <optgroup label="Africa">
    <option value="eg">Egypt</option>
    <option value="ma">Morocco</option>
  </optgroup>
  <optgroup label="Europe">
    <option value="fr">France</option>
  </optgroup>
</select>
```

**🔗 Follow-up:**
_Can a user select multiple options?_
**↳ Answer:**
Yes. The `<select>` element can have the `multiple` attribute.

---

### 📌 Q49 — What is the difference between `checked`, `selected`, and `value`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

1. **`checked`** is used with checkbox and radio inputs to indicate their default checked state.
2. **`selected`** is used on an `<option>` to indicate its default selected state.
3. **`value`** specifies the value associated with a form control.

**🔗 Follow-up:**
_Does `checked` mean the checkbox can never be unchecked?_
**↳ Answer:**
No. It represents the initial/default checked state. The user can normally change it unless the control is disabled or otherwise restricted.

---

### 📌 Q50 — What is HTML form validation, and why is it useful?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
HTML provides built-in client-side validation through attributes such as:

1. `required`
2. `minlength`
3. `maxlength`
4. `min`
5. `max`
6. `pattern`
7. input types such as `email`

However, client-side validation should not be considered a security boundary. The backend must validate the data again because the client can be bypassed or manipulated.

**🔗 Follow-up:**
_If Angular Reactive Forms validates the email, do we still need backend validation?_
**↳ Answer:**
Absolutely. Frontend validation improves user experience and provides immediate feedback, but backend validation is required for security and data integrity because clients cannot be trusted.

---

### 📌 Q51 — What is the difference between `<form>` and `<fieldset>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`<form>` represents a complete form that contains controls and can be submitted.
`<fieldset>` is used to group related form controls together semantically.

**🔗 Follow-up:**
_What is the purpose of `<legend>`?_
**↳ Answer:** `<legend>` provides a caption or accessible name for the `<fieldset>`.

---

### 📌 Q52 — What is the difference between client-side and server-side validation?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Client-side validation happens in the browser before the request is sent to the server. It provides fast feedback and improves user experience.
Server-side validation happens on the backend and is essential because the client cannot be trusted.

**🔗 Follow-up:**
_Why can't we rely only on Angular validation?_
**↳ Answer:**
Because a user can bypass the Angular application entirely and send requests directly to the API using tools such as Postman or custom scripts.

---

### 📌 Q53 — What is the difference between `<input type="submit">` and `<button type="submit">`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Both can submit a form when they're associated with a form.
`<input type="submit">` is an input control whose displayed content is controlled through its `value`.
`<button type="submit">` is a button element whose content can contain text and, depending on the allowed content, richer markup.

**🔗 Follow-up:**
_What is the default type of a `<button>` inside a form?_
**↳ Answer:**
The default behavior is submit, so it's good practice to explicitly specify the type.

---

### 📌 Q54 — What is the difference between `type="button"` and `type="submit"`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`type="submit"` submits the associated form.
`type="button"` is a normal button and doesn't submit the form by default.

**🔗 Follow-up:**
_What would you use for opening a modal?_
**↳ Answer:**
Usually: `<button type="button">Open Modal</button>` because opening a modal is an action, not a form submission.

---

### 📌 Q55 — What happens when an HTML form is submitted?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
When a form is submitted, the browser identifies the successful form controls, constructs the form data, and depending on the form's method and action, sends a request to the specified URL.

**🔗 Follow-up:**
_What happens to disabled form controls during native submission?_
**↳ Answer:**
Disabled controls are generally not included in the submitted form data.

---

### 📌 Q56 — What are "successful controls" in HTML forms?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Successful controls are form controls whose names and values are included when the browser constructs the form data for submission.
For example, a disabled input is generally not successful and won't be included. Checkboxes that are not checked are also generally not included. Controls typically need an appropriate `name` to contribute a name-value pair.

**🔗 Follow-up:**
_If I have `<input type="checkbox" name="active" value="true">` and it's unchecked, will `active=false` automatically be submitted?_
**↳ Answer:**
No. An unchecked checkbox is generally not included in native form submission at all. If the backend needs an explicit `false`, the application needs to handle that appropriately.

---

### 📌 Q57 — What is the `action` attribute of a `<form>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
The `action` attribute specifies the URL where the form submission should be sent.

**🔗 Follow-up:**
_What happens if `action` isn't specified?_
**↳ Answer:**
The form submits to the current document's URL by default.

---

### 📌 Q58 — What is the difference between `GET` and `POST` in HTML forms?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
With a GET form submission, the form data is encoded into the URL query string.
With POST, the form data is sent in the request body.

**🔗 Follow-up:**
_Can GET requests modify data?_
**↳ Answer:**
Technically a server could be implemented that way, but according to HTTP semantics, GET should be safe and used for retrieving representations rather than performing state-changing operations.

---

### 📌 Q59 — What is HTML escaping and why is it important?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
HTML escaping converts special characters into safe HTML representations so that user-provided text isn't interpreted as HTML markup.
For example:

- `<` → `&lt;`
- `>` → `&gt;`
- `&` → `&amp;`

This is important when displaying untrusted content because it can help prevent HTML injection and XSS vulnerabilities.

**🔗 Follow-up:**
_Is escaping alone enough to prevent all XSS?_
**↳ Answer:**
No. XSS prevention depends on the context and proper output encoding, safe APIs, sanitization where appropriate, and framework protections. Different contexts such as HTML, JavaScript, CSS, and URLs require different handling.

---

### 📌 Q60 — What is XSS?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
XSS, or Cross-Site Scripting, is a vulnerability where an attacker manages to cause malicious JavaScript or other executable content to run in another user's browser in the context of a trusted website.
There are several types, including:

1. Stored XSS
2. Reflected XSS
3. DOM-based XSS

**🔗 Follow-up:**
_Does Angular protect against XSS?_
**↳ Answer:**
Angular provides built-in protections by escaping/interpreting template-bound values safely and sanitizing certain potentially dangerous values and contexts. However, developers can still introduce vulnerabilities by bypassing Angular's security mechanisms, using unsafe DOM APIs, or incorrectly trusting/sanitizing untrusted content.

**🔗 Follow-up 2:**
_What is the danger of using `innerHTML` with user input?_
**↳ Answer:**
If untrusted input is inserted as HTML without proper sanitization, an attacker may inject malicious markup or scripts, creating an XSS vulnerability.

---

### 📌 Q61 — What is the difference between `class` and `id` in CSS and JavaScript?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
An `id` is intended to uniquely identify one element, while a `class` can be shared by multiple elements.
In CSS: `#header { }` vs `.card { }`
In JS: `document.getElementById('header')` vs `document.querySelector('.card')`

**🔗 Follow-up:**
_Can an element have multiple classes?_
**↳ Answer:** Yes. `<div class="card active featured"></div>`

---

### 📌 Q62 — What is the difference between `name` and `id` in HTML forms?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`id` uniquely identifies an element in the document and can be used to associate a `<label>` with a form control.
`name` identifies the form control when its data is included in native form submission.

**🔗 Follow-up:**
_Can two inputs have the same `name`?_
**↳ Answer:** Yes. This is common with radio buttons, where multiple options share the same name.

---

### 📌 Q63 — What is the difference between `<figure>` and `<img>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`<img>` represents an image.
`<figure>` is a semantic container for self-contained content such as an image, diagram, code example, or illustration, optionally accompanied by a `<figcaption>`.

**🔗 Follow-up:**
_Is `<figure>` only for images?_
**↳ Answer:** No. It can represent other self-contained content, such as diagrams, charts, code snippets, or illustrations.

---

### 📌 Q64 — What is the purpose of `<figcaption>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<figcaption>` provides a caption or description for the content inside a `<figure>`.

**🔗 Follow-up:**
_Can `<figcaption>` appear before the image?_
**↳ Answer:** Yes. It can appear as the first or last child of `<figure>`.

---

### 📌 Q65 — What is the difference between `<video>` and `<audio>`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
`<video>` is used to embed video content, while `<audio>` is used for audio content. Both support common attributes such as `controls`, `autoplay`, `loop`, `muted`, `preload`.

**🔗 Follow-up:**
_Why might `autoplay` fail even if I specify `autoplay`?_
**↳ Answer:** Modern browsers often restrict `autoplay` when media contains audio or isn't considered user-initiated. Muted `autoplay` is more commonly allowed.

---

### 📌 Q66 — What is the purpose of the `<source>` element?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`<source>` specifies alternative media resources for elements such as `<video>` and `<audio>`. The browser can choose a supported source format.

**🔗 Follow-up:**
_What happens if none of the sources are supported?_
**↳ Answer:** The browser won't be able to play the media, and fallback content placed inside the `<video>` or `<audio>` element can be displayed.

---

### 📌 Q67 — What is the difference between `<canvas>` and `<svg>`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**  
`<canvas>` provides a bitmap drawing surface that JavaScript can manipulate, while SVG is a vector-based markup format where graphical elements are represented as DOM nodes.
Canvas is often useful for games, image processing, etc. SVG is useful for scalable graphics, icons, diagrams.

**🔗 Follow-up:**
_Which one scales without losing quality?_
**↳ Answer:** SVG is vector-based, so it scales without the pixelation associated with bitmap graphics.

**🔗 Follow-up 2:**
_Can I style SVG elements with CSS?_
**↳ Answer:** Yes, SVG elements can often be styled and manipulated using CSS and JavaScript.

---

### 📌 Q68 — What is the difference between `<template>` and normal HTML elements?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
The `<template>` element contains HTML that isn't rendered as part of the document immediately. Its content is stored as a `DocumentFragment` and can later be cloned and inserted into the DOM using JavaScript.

**🔗 Follow-up:**
_Is the content inside `<template>` immediately visible?_
**↳ Answer:** No. It's inert until it is explicitly cloned and inserted into the document.

---

### 📌 Q69 — What is the `contenteditable` attribute?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`contenteditable` makes an element's content editable by the user.

**🔗 Follow-up:**
_Would you trust the content entered through `contenteditable` and send it directly to the backend?_
**↳ Answer:** No. User-generated content must be treated as untrusted. If it's stored or rendered as HTML, it needs appropriate validation/sanitization to avoid XSS.

---

### 📌 Q70 — What is the `tabindex` attribute and why is it important?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**  
`tabindex` controls whether an element can receive keyboard focus and, in some cases, its position in the sequential keyboard navigation order.

- `0`: participates in natural tab order.
- `-1`: allows programmatic focus but removes from sequential keyboard navigation.

**🔗 Follow-up:**
_Should we use positive `tabindex` values like `tabindex="1"`?_
**↳ Answer:** Generally no. Positive values create a custom tab order that can become difficult to maintain and harm accessibility. Rely on natural document order.

---

### 📌 Q71 — What is the difference between `autocomplete="on"` and specific autocomplete tokens?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`autocomplete="on"` allows general autofill. Specific tokens (e.g., `email`, `username`, `new-password`) give precise information to improve autofill accuracy and password manager behavior.

**🔗 Follow-up:**
_Why is `autocomplete="new-password"` useful?_
**↳ Answer:** It tells the browser the field is for a new password, helping password managers behave appropriately.

---

### 📌 Q72 — What is the purpose of the `accept` attribute on `<input type="file">`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
The `accept` attribute provides a hint to the browser about the types of files the user should select (e.g., `accept="image/*"`). It helps filter the file picker.

**🔗 Follow-up:**
_Does `accept` guarantee that the uploaded file is actually an image?_
**↳ Answer:** No. It's only a client-side hint. The backend must validate the uploaded file independently.

---

### 📌 Q73 — What is the difference between `multipart/form-data` and `application/x-www-form-urlencoded`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `application/x-www-form-urlencoded` encodes form fields as key-value pairs in the request body using URL encoding.
- `multipart/form-data` divides the request body into multiple parts, making it suitable for uploading files along with regular form fields.

**🔗 Follow-up:**
_Why wouldn't we normally send a file using JSON?_
**↳ Answer:** JSON isn't designed to represent binary file data directly. `multipart/form-data` is designed specifically for sending files and fields together.

---

### 📌 Q74 — What is the difference between `enctype="application/x-www-form-urlencoded"` and `enctype="multipart/form-data"` in a form?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
The `enctype` attribute determines how the browser encodes form data. `multipart/form-data` is used for file uploads. `application/x-www-form-urlencoded` is the default for ordinary text data.

**🔗 Follow-up:**
_If a form contains an image upload, which `enctype` would you choose?_
**↳ Answer:** `multipart/form-data`.

---

### 📌 Q75 — What is the purpose of the `novalidate` attribute on a form?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`novalidate` tells the browser not to perform its built-in constraint validation when submitting the form. Useful when handling validation entirely through JS/Frameworks.

**🔗 Follow-up:**
_Does `novalidate` remove Angular Reactive Forms validators?_
**↳ Answer:** No. It affects native HTML validation. Angular's validation system is separate and still runs.

---

### 📌 Q76 — What is the difference between `minlength` and `pattern`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`minlength` checks character count. `pattern` uses a regular expression to define a required format.

**🔗 Follow-up:**
_Does `minlength` validate that a value exists?_
**↳ Answer:** Not necessarily. If optional, empty is allowed. Use `required` to enforce existence.

---

### 📌 Q77 — What is the difference between `min/max` and `minlength/maxlength`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`min` and `max` constrain numerical values. `minlength` and `maxlength` constrain character counts in text inputs.

**🔗 Follow-up:**
_What if I use `min="8"` on a text input?_
**↳ Answer:** `min` isn't a string-length validator. Use `minlength` for text.

---

### 📌 Q78 — What is the purpose of the `loading` attribute on images and iframes?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
The `loading` attribute hints when resources should load. `lazy` defers loading until near the viewport. `eager` loads immediately.

**🔗 Follow-up:**
_Should every image use `loading="lazy"`?_
**↳ Answer:** Not necessarily. Important above-the-fold images (like LCP) should be loaded eagerly.

---

### 📌 Q79 — What is the `srcset` attribute and why is it useful?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`srcset` allows providing multiple image resources so the browser can choose based on viewport size/density, reducing bandwidth usage.

**🔗 Follow-up:**
_What's the difference between `srcset` and `sizes`?_
**↳ Answer:** `srcset` provides candidates. `sizes` tells the browser the expected rendered width under different conditions to help it choose.

---

### 📌 Q80 — What is the difference between `srcset` and `<picture>`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`srcset` chooses based on resolution/size. `<picture>` provides more control, including media conditions, different formats, and art direction.

**🔗 Follow-up:**
_When would you use `<picture>` instead of only `srcset`?_
**↳ Answer:** When needing art direction, media-based source selection, or different image formats (like WebP).

---

### 📌 Q81 — What is the difference between `block`, `inline`, and `inline-block` elements?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**

- **`block`**: starts on a new line, takes available width.
- **`inline`**: flows within text, doesn't accept width/height.
- **`inline-block`**: flows inline but accepts width/height.

**🔗 Follow-up:**
_Is `<div>` always block and `<span>` always inline?_
**↳ Answer:** By default, yes. But CSS `display` property can change their behavior.

---

### 📌 Q82 — What is the difference between `width: 100%` and `width: 100vw`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`width: 100%` occupies 100% of the containing block. `100vw` is 100% of the viewport width.

**🔗 Follow-up:**
_Why can `100vw` sometimes cause horizontal scrolling?_
**↳ Answer:** Because `vw` includes the scrollbar area, making the element slightly wider than the available layout area.

---

### 📌 Q83 — What is the difference between `em`, `rem`, `%`, `vh`, and `vw`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- **`px`**: absolute CSS pixel.
- **`%`**: relative to containing dimension.
- **`em`**: relative to element's (or parent's) font size.
- **`rem`**: relative to root element's font size.
- **`vh` / `vw`**: relative to viewport height/width.

**🔗 Follow-up:**
_Why is `rem` often preferred over `em` for consistent sizing?_
**↳ Answer:** `rem` is based on the root font size, avoiding compounding behavior of nested `em` values.

---

### 📌 Q84 — What is the CSS box model?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Describes how dimensions are composed: Content → Padding → Border → Margin.

**🔗 Follow-up:**
_What is the difference between `content-box` and `border-box`?_
**↳ Answer:** `content-box` (default) applies width/height to content only. `border-box` includes content, padding, and border in the declared dimensions.

---

### 📌 Q85 — What is the difference between margin collapsing and padding?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Padding is inside the element. Margin is outside. Vertical margins between certain block-level elements can collapse (combine into the larger margin, rather than adding up).

**🔗 Follow-up:**
_Does padding collapse?_
**↳ Answer:** No. Padding doesn't participate in margin collapsing.

---

### 📌 Q86 — What is CSS specificity?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
The algorithm to determine which selector wins. Hierarchy: Inline styles → IDs → Classes/attributes/pseudo-classes → Elements/pseudo-elements.

**🔗 Follow-up:**
_What is `!important`?_
**↳ Answer:** Changes priority in the cascade. Use sparingly as it makes CSS hard to maintain.

---

### 📌 Q87 — What is the difference between pseudo-class and pseudo-element?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- **Pseudo-class** (`:hover`, `:focus`): represents a state or condition.
- **Pseudo-element** (`::before`, `::first-letter`): represents a specific part of an element or generated content.

---

### 📌 Q88 — What is a stacking context, and how is it related to `z-index`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
A conceptual group of elements painted together. `z-index` controls stacking within the context. A child cannot escape its parent's stacking context just by using a huge `z-index`.

---

### 📌 Q89 — What is the difference between reflow and repaint?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- **Reflow (Layout)**: recalculating geometry/position (e.g., changing `width`).
- **Repaint**: redrawing pixels without recalculating layout (e.g., changing `background-color`).

**🔗 Follow-up:**
_Why are `transform` and `opacity` preferred for animations?_
**↳ Answer:** They are handled efficiently during compositing, avoiding repeated layout calculations.

---

### 📌 Q90 — What is the Critical Rendering Path?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
The sequence: HTML → DOM → CSS → CSSOM → Render Tree → Layout → Paint → Compositing. JS can block parsing; CSS blocks rendering.

---

### 📌 Q91 — What is the difference between HTML parsing and DOM construction?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
HTML parsing reads tokens. DOM construction builds the in-memory tree representation. The DOM can be modified by JS, so it differs from the original source.

---

### 📌 Q92 — What happens if the browser encounters malformed HTML?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Browsers are fault-tolerant. They use error-recovery rules to construct a valid DOM tree (e.g., auto-closing tags).

---

### 📌 Q93 — What is the DOM, and why is it important for JavaScript?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Object-based representation of HTML. JS uses it to find, change, create, remove elements, and respond to events.

---

### 📌 Q94 — What is event bubbling?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Event propagates upward from the target element through its ancestors. Stopped via `event.stopPropagation()`.

---

### 📌 Q95 — What is event capturing?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Event travels from outer ancestors down to the target before the target phase. Registered using `{ capture: true }` in `addEventListener`.

---

### 📌 Q96 — What is event delegation?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Attaching a single event listener to a parent instead of many children, relying on event bubbling. Reduces memory overhead and handles dynamic children easily.

---

### 📌 Q97 — What is the difference between `event.target` and `event.currentTarget`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `event.target`: element where the event originated.
- `event.currentTarget`: element whose listener is currently executing.

---

### 📌 Q98 — What is the difference between `preventDefault()` and `stopPropagation()`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**

- `preventDefault()`: stops default browser action (e.g., form submit).
- `stopPropagation()`: stops event propagation through the DOM.

---

### 📌 Q99 — What is Shadow DOM?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Web platform feature allowing an element to have an encapsulated DOM subtree and styles, isolated from the main document.

---

### 📌 Q100 — What is Web Accessibility, and how would you make an HTML page accessible?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Designing for all abilities. Focus on: Semantic HTML, proper labels, keyboard accessibility, meaningful alt text, focus management, ARIA when necessary, color contrast, and accessible forms.

---

---

# 🎨 CSS Mastery

### 📌 Q1 — What is CSS and what problem does it solve?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
CSS (Cascading Style Sheets) controls presentation and layout (colors, fonts, spacing, responsive design, animations). HTML is structure; CSS is presentation.

---

### 📌 Q2 — What does "Cascading" mean in CSS?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
The process to determine which declarations apply when multiple rules target the same element. Depends on origin/importance, cascade layers, specificity, and source order.

---

### 📌 Q3 — What are the three main ways to apply CSS?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

1. Inline (`style="..."`)
2. Internal (`<style>`)
3. External (`<link rel="stylesheet">`) - Preferred for maintainability.

---

### 📌 Q4 — What is a CSS selector?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Identifies elements to apply rules to. Types: element, class, ID, attribute, combinators, pseudo-classes, pseudo-elements.

---

### 📌 Q5 — What is the difference between `*`, element, class, and ID selectors?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

- `*`: Universal (all elements).
- `p`: Element (all `<p>`).
- `.card`: Class (elements with `class="card"`).
- `#header`: ID (element with that specific ID).

---

### 📌 Q6 — What is the difference between descendant and child selectors?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- Descendant (space `.container p`): any `<p>` inside `.container`.
- Child (`>` `.container > p`): only direct child `<p>` of `.container`.

---

### 📌 Q7 — What is the difference between `:first-child`, `:first-of-type`, and `:nth-child()`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `:first-child`: first child of parent, regardless of type.
- `:first-of-type`: first sibling of that specific element type.
- `:nth-child(n)`: based on position among all children.

---

### 📌 Q8 — What is CSS inheritance?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Some properties (color, font-family) automatically take their value from the ancestor. Others (margin, padding, border) do not.

---

### 📌 Q9 — What is the difference between `inherit`, `initial`, `unset`, and `revert`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `inherit`: forces taking parent's value.
- `initial`: resets to CSS-defined initial value.
- `unset`: acts as `inherit` for inherited props, `initial` for non-inherited.
- `revert`: rolls back to previous cascade level (browser/user defaults).

---

### 📌 Q10 — What is the difference between `display: none`, `visibility: hidden`, and `opacity: 0`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `display: none`: removed from layout, takes no space.
- `visibility: hidden`: invisible, but keeps layout space.
- `opacity: 0`: fully transparent, keeps space, can still be interactive.

---

### 📌 Q11 — What is the difference between `content-box` and `border-box`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
`content-box` (default): width/height apply to content only.
`border-box`: width/height include content, padding, and border.

---

### 📌 Q12 — What does `box-sizing: border-box` solve?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Makes width/height calculations predictable. Commonly applied globally (`* { box-sizing: border-box; }`).

---

### 📌 Q13 — Explain `position: static`, `relative`, `absolute`, `fixed`, and `sticky`.

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `static`: default, normal flow.
- `relative`: normal flow, but can be visually offset. Establishes containing block.
- `absolute`: removed from flow, positioned relative to containing block.
- `fixed`: removed from flow, positioned relative to viewport.
- `sticky`: behaves like relative until scroll threshold, then sticks.

---

### 📌 Q14 — What is the difference between `relative` positioning and `absolute` positioning?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`relative` keeps element in normal flow (reserves space). `absolute` removes it from flow (doesn't reserve space).

---

### 📌 Q15 — What is `overflow`, and what is the difference between `visible`, `hidden`, `scroll`, and `auto`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Controls content exceeding the box.

- `visible`: extends outside.
- `hidden`: clipped.
- `scroll`: always shows scrollbars.
- `auto`: shows scrollbars only when needed.

---

### 📌 Q16 — What is the difference between `overflow: hidden` and `clip`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Both clip content. `overflow: hidden` can create a scroll container. `overflow: clip` strictly clips without providing scrolling behavior.

---

### 📌 Q17 — What is margin collapsing?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Vertical margins of certain block-level elements combine (take the larger value) rather than adding together.

---

### 📌 Q18 — What is a Block Formatting Context (BFC)?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Layout context where block-level boxes are laid out. Affects float interaction, margin collapsing, and containment. Created via `display: flow-root`, flex, grid, etc.

---

### 📌 Q19 — What was the traditional `clearfix` technique used for?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Used `::after` pseudo-element with `clear: both` to force a parent to contain its floated children. Modern layouts prefer Flexbox/Grid or `display: flow-root`.

---

### 📌 Q20 — What is Flexbox and when would you use it?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
One-dimensional layout system (row or column). Used for nav bars, aligning items, centering, distributing space.

---

### 📌 Q21 — What is the difference between `justify-content`, `align-items`, and `align-content` in Flexbox?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `justify-content`: distributes items along the **main axis**.
- `align-items`: aligns items along the **cross axis** within a line.
- `align-content`: distributes **multiple lines** along the cross axis.

---

### 📌 Q22 — What is the difference between `align-items` and `align-self`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`align-items` is set on the container (default for all items). `align-self` is set on an individual item to override the container's setting.

---

### 📌 Q23 — What is the difference between `flex-grow`, `flex-shrink`, and `flex-basis`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `flex-grow`: how much it grows when extra space is available.
- `flex-shrink`: how much it shrinks when space is lacking.
- `flex-basis`: initial main-size before space distribution.

---

### 📌 Q24 — What is the difference between `flex-basis: auto` and `flex-basis: 0`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`auto`: uses the item's width/height as basis.
`0`: basis is zero, so free space is distributed purely based on `flex-grow`.

---

### 📌 Q25 — What does `min-width: 0` solve in Flexbox?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Flex items have an automatic minimum size (content size) that can prevent shrinking. `min-width: 0` allows them to shrink below their content's intrinsic size, preventing overflow.

---

### 📌 Q26 — What is the difference between `gap`, `margin`, and `padding` in a Flexbox layout?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `gap`: consistent spacing **between** items.
- `margin`: space outside an individual element.
- `padding`: space inside an element, between content and border.

---

### 📌 Q27 — What is CSS Grid, and how is it different from Flexbox?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Grid is a **two-dimensional** layout system (rows and columns). Flexbox is **one-dimensional** (row OR column).

---

### 📌 Q28 — What does `fr` mean in CSS Grid?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Fractional unit. Represents a fraction of the available space in the grid container.

---

### 📌 Q29 — What is the difference between `auto-fit` and `auto-fill` in CSS Grid?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `auto-fit`: collapses empty tracks, allowing existing items to expand.
- `auto-fill`: keeps empty tracks if they fit.

---

### 📌 Q30 — What is `minmax()` in CSS Grid?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**  
Defines a minimum and maximum size for a grid track. E.g., `minmax(250px, 1fr)`. Great for responsive layouts without media queries.

---

### 📌 Q31 — What is the difference between `grid-template-columns` and `grid-auto-columns`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`grid-template-columns`: explicitly defined columns.
`grid-auto-columns`: size of implicitly created columns.

---

### 📌 Q32 — What is the difference between `grid-template-rows` and `grid-auto-rows`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`grid-template-rows`: explicitly defined rows.
`grid-auto-rows`: size of implicitly created rows.

---

### 📌 Q33 — What is the difference between `grid-column`, `grid-row`, and `grid-area`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `grid-column`: start/end across columns.
- `grid-row`: start/end across rows.
- `grid-area`: shorthand for row-start/col-start/row-end/col-end, or named areas.

---

### 📌 Q34 — What is `grid-template-areas` and when would you use it?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Defines named regions using a visual string representation. Makes complex page layouts highly readable.

---

### 📌 Q35 — What is the difference between `justify-items`, `align-items`, `justify-content`, and `align-content` in CSS Grid?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `justify-items` / `align-items`: aligns **items** within their grid areas.
- `justify-content` / `align-content`: distributes the **entire grid tracks** when there is extra space.

---

### 📌 Q36 — What is the difference between `justify-self` and `justify-items`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`justify-items`: set on container, default for all items.
`justify-self`: set on individual item, overrides container.

---

### 📌 Q37 — What is a media query?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Applies CSS conditionally based on environment characteristics (e.g., viewport width).

---

### 📌 Q38 — What is mobile-first responsive design?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Designing base styles for small screens first, then using `min-width` media queries to progressively enhance for larger screens.

---

### 📌 Q39 — What is the difference between `min-width` and `max-width` media queries?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`min-width`: applies when viewport is **at least** X wide (mobile-first).
`max-width`: applies when viewport is **at most** X wide (desktop-first).

---

### 📌 Q40 — What are CSS functions such as `calc()`, `min()`, `max()`, and `clamp()`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**

- `calc()`: arithmetic expressions.
- `min()`: chooses smallest value.
- `max()`: chooses largest value.
- `clamp(min, preferred, max)`: fluid scaling within limits.

---

### 📌 Q41 — What is CSS specificity, and how is it calculated?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Mechanism to determine selector priority. Inline > IDs > Classes/Attributes/Pseudo-classes > Elements/Pseudo-elements.

---

### 📌 Q42 — Which is more specific: `#id`, `.class`, `[attribute]`, `:hover`, or `div`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
`#id` > `.class` = `[attribute]` = `:hover` > `div`.

---

### 📌 Q43 — What does `!important` do, and why should you avoid overusing it?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Increases cascade priority. Overusing it makes overriding styles difficult and creates maintenance nightmares.

---

### 📌 Q44 — What is a CSS custom property?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
User-defined property storing reusable values (e.g., `--primary-color: blue;`). Defined on `:root` for global scope. Used via `var()`.

---

### 📌 Q45 — What is the difference between CSS variables and Sass variables?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Sass variables (`$primary`) are processed at compile time. CSS custom properties (`--primary`) exist at runtime in the browser, can be changed dynamically, and participate in the cascade.

---

### 📌 Q46 — What is a stacking context, and how is it related to `z-index`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Conceptual layering context. `z-index` is evaluated within it. Created by positioned elements with non-auto z-index, opacity < 1, transforms, etc.

---

### 📌 Q47 — How can `transform` affect `z-index` or stacking behavior?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Applying a `transform` creates a new stacking context, constraining the `z-index` of its descendants.

---

### 📌 Q48 — What is the difference between a CSS transition and a CSS animation?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**

- **Transition**: animates property change between two states (requires state change).
- **Animation**: uses `@keyframes` to define multiple stages, can run automatically.

---

### 📌 Q49 — Why is `transform: translate()` often preferred over changing `top` or `left` for animations?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
`transform` avoids triggering layout recalculation (reflow), resulting in smoother, GPU-accelerated animations.

---

### 📌 Q50 — What is the difference between `em`, `rem`, `%`, `vw`, and `vh`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `rem`: root font size.
- `em`: element/parent font size.
- `%`: containing dimension.
- `vw`/`vh`: viewport width/height.

---

### 📌 Q51 — What is the difference between a pseudo-class and a pseudo-element?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Pseudo-class (`:hover`): state/condition. Pseudo-element (`::before`): part of element/generated content.

---

### 📌 Q52 — What is the difference between `::before` and `::after`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
`::before` inserts as first child. `::after` inserts as last child. Both require the `content` property. Not real DOM nodes.

---

### 📌 Q53 — What is the difference between `:nth-child()` and `:nth-of-type()`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`:nth-child()`: counts all siblings.
`:nth-of-type()`: counts only siblings of the same element type.

---

### 📌 Q54 — What is the difference between `:not()`, `:is()`, and `:where()`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `:not()`: matches elements NOT matching the selector.
- `:is()`: groups selectors, takes specificity of most specific argument.
- `:where()`: groups selectors, but always has **zero specificity**.

---

### 📌 Q55 — What does the CSS `:has()` pseudo-class do?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Selects an element based on whether it contains a matching descendant (often called a "parent selector"). E.g., `.card:has(img)`.

---

### 📌 Q56 — What does `currentColor` mean in CSS?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Represents the element's computed `color` value. Useful for inheriting text color in borders or SVG fills.

---

### 📌 Q57 — What is `object-fit`, and why is it useful for images?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Controls how replaced content (image/video) fits in its box.

- `cover`: fills box, preserves aspect ratio, may crop.
- `contain`: fits entirely, preserves aspect ratio, may leave empty space.

---

### 📌 Q58 — What is the difference between `object-fit` and `background-size: cover`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`object-fit` is for `<img>`/`<video>` tags (semantic content). `background-size` is for CSS background images (decorative).

---

### 📌 Q59 — What is `aspect-ratio` and why is it useful?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Defines preferred width-to-height ratio. Prevents layout shifts and maintains consistent dimensions for media containers.

---

### 📌 Q60 — What is `will-change`, and why shouldn't it be overused?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
Hints to the browser to optimize for upcoming changes. Overusing it wastes memory and rendering resources. Use selectively.

---

### 📌 Q61 — Explain the CSS Box Model.

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Content → Padding → Border → Margin. Default `content-box` applies width to content only. `border-box` includes padding and border.

---

### 📌 Q62 — What is the difference between `content-box` and `border-box`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`content-box`: width/height = content.
`border-box`: width/height = content + padding + border. (Margin is always outside).

---

### 📌 Q63 — What is margin collapsing?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Vertical margins of adjacent block-level elements combine into a single margin equal to the largest of the two.

---

### 📌 Q64 — What is the difference between `display: none`, `visibility: hidden`, and `opacity: 0`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `display: none`: removed from layout.
- `visibility: hidden`: invisible, keeps space, removed from accessibility tree.
- `opacity: 0`: transparent, keeps space, can still be interactive.

---

### 📌 Q65 — Explain the CSS `position` values: `static`, `relative`, `absolute`, `fixed`, and `sticky`.

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `static`: default.
- `relative`: offset from normal position, establishes containing block.
- `absolute`: removed from flow, relative to containing block.
- `fixed`: relative to viewport.
- `sticky`: relative until scroll threshold.

---

### 📌 Q66 — How does `position: sticky` actually work?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Participates in normal flow, then sticks relative to its scrolling container when reaching a threshold (e.g., `top: 0`). Fails if ancestors have specific overflow settings.

---

### 📌 Q67 — What is the difference between `overflow: hidden`, `auto`, `scroll`, and `clip`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**

- `hidden`: clips, no scrollbars.
- `auto`: scrollbars if needed.
- `scroll`: always shows scrollbars.
- `clip`: clips strictly, no scrolling mechanism.

---

### 📌 Q68 — What is the difference between `display: block`, `inline`, and `inline-block`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

- `block`: new line, takes width.
- `inline`: flows with text, no width/height.
- `inline-block`: flows with text, accepts width/height.

---

### 📌 Q69 — What is the difference between `overflow-wrap`, `word-break`, and `white-space`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `overflow-wrap`: breaks unbreakable strings to prevent overflow.
- `word-break`: controls how words break across lines.
- `white-space`: controls whitespace handling and line wrapping (e.g., `nowrap`).

---

### 📌 Q70 — What is the difference between `overflow: hidden` and text truncation with ellipsis?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`overflow: hidden` just clips. For ellipsis (`...`), use:

```css
white-space: nowrap;
overflow: hidden;
text-overflow: ellipsis;
```

---

### 📌 Q71 — What is the CSS Cascade?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Algorithm determining which rules win. Factors: Origin/Importance → Layers → Specificity → Source Order.

---

### 📌 Q72 — What is CSS inheritance?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Properties like `color` and `font-family` automatically pass to children. `margin` and `padding` do not.

---

### 📌 Q73 — What do `inherit`, `initial`, `unset`, and `revert` mean?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `inherit`: from parent.
- `initial`: CSS default.
- `unset`: inherit if inheritable, else initial.
- `revert`: rolls back to previous cascade origin.

---

### 📌 Q74 — What is the difference between `:focus`, `:focus-visible`, and `:focus-within`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**

- `:focus`: whenever focused.
- `:focus-visible`: only when keyboard focus is appropriate.
- `:focus-within`: when the element or any descendant has focus.

---

### 📌 Q75 — What is `prefers-reduced-motion` and why is it important?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Media feature detecting user's OS preference for reduced motion. Crucial for accessibility to prevent discomfort from animations.

---

### 📌 Q76 — What is the difference between `display: flex` and `display: inline-flex`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Both create flex contexts for children. `flex` makes the container block-level. `inline-flex` makes it inline-level.

---

### 📌 Q77 — What is `display: contents`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Removes the element's own CSS box from layout, allowing its children to participate in the parent's layout as if the wrapper didn't exist.

---

### 📌 Q78 — What is `contain` in CSS?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Limits how an element's layout, paint, size, or style affects the rest of the page. Improves performance by isolating rendering work.

---

### 📌 Q79 — What is the difference between `visibility: collapse` and `visibility: hidden`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`hidden`: invisible, keeps space.
`collapse`: designed for table rows/columns to collapse them while preserving table layout characteristics.

---

### 📌 Q80 — What is CSS `@supports`, and how can it help with progressive enhancement?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Conditionally applies rules based on browser feature support. Enables graceful fallbacks and progressive enhancement.

---

### 📌 Q81 — What is the difference between `reflow` (layout) and `repaint`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- **Reflow**: recalculates geometry (expensive).
- **Repaint**: redraws pixels (cheaper).
  `transform` avoids reflow.

---

### 📌 Q82 — What is compositing in browser rendering?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Divides content into layers and composites them. `transform` and `opacity` are handled here, making them ideal for animations.

---

### 📌 Q83 — What are CSS logical properties, and why are they useful?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Describe dimensions based on writing direction (e.g., `margin-inline-start` instead of `margin-left`). Essential for RTL/LTR support.

---

### 📌 Q84 — What is the difference between `direction: ltr/rtl` and `dir="ltr/rtl"`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`dir` is an HTML attribute (semantic/document-level). `direction` is a CSS property. Use HTML `dir` for document direction, CSS logical properties for styling.

---

### 📌 Q85 — How do you make a CSS form accessible?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Combine semantic HTML with CSS: associate labels, ensure visible focus states, don't rely on color alone for errors, maintain contrast, ensure keyboard navigation works.

---

### 📌 Q86 — What is `accent-color` in CSS?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Customizes the accent color of native form controls (checkboxes, radios) while keeping native behavior.

---

### 📌 Q87 — What are responsive images, and why are `srcset` and `sizes` useful?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
`srcset` provides image candidates. `sizes` tells the browser expected rendered width. Saves bandwidth by downloading appropriately sized images.

---

### 📌 Q88 — What is `object-position`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Controls the position of replaced content (like an image) within its box, especially useful with `object-fit: cover` to decide which part is cropped.

---

### 📌 Q89 — What is CSS nesting?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Allows selectors to be nested inside another rule natively in CSS. Similar to Sass, but processed by the browser.

---

### 📌 Q90 — How would you organize CSS in a large Angular application?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Separate by responsibility: Global (tokens, reset, utilities), Components (local styles), Pages/Layouts. Avoid massive global stylesheets. Use design tokens and consistent naming.

---

### 📌 Q91 — What are CSS Custom Properties, and how are they different from Sass variables?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
CSS Custom Properties (`--var`) are runtime, inheritable, and cascade-aware. Sass variables (`$var`) are compile-time only.

---

### 📌 Q92 — What is CSS `calc()` and when would you use it?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**  
Performs math in CSS. E.g., `width: calc(100% - 40px)`. Useful for mixing units.

---

### 📌 Q93 — What is the difference between `min()`, `max()`, and `clamp()`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `min()`: smallest value.
- `max()`: largest value.
- `clamp(min, preferred, max)`: fluid scaling bounded by min and max.

---

### 📌 Q94 — What is a CSS Cascade Layer (`@layer`)?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
Explicitly organizes CSS into layers to control precedence, reducing the need for specificity hacks. E.g., `@layer reset, components, utilities;`.

---

### 📌 Q95 — What is `!important`, and why should it generally be avoided?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Overrides cascade priority. Creates maintenance nightmares. Solve issues using specificity, layers, or better selectors instead.

---

### 📌 Q96 — What is the difference between CSS transitions and animations?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Transitions animate between two states (requires trigger). Animations use `@keyframes` for complex, multi-step sequences that can run automatically.

---

### 📌 Q97 — What are CSS animation `keyframes`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
Define intermediate states of an animation using percentages or `from`/`to`.

---

### 📌 Q98 — What is the difference between `em`, `rem`, `%`, `vw`, `vh`, and `px`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- `px`: absolute.
- `rem`: root font size.
- `em`: element font size.
- `%`: parent dimension.
- `vw`/`vh`: viewport dimensions.

---

### 📌 Q99 — How do media queries work, and what is mobile-first CSS?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Media queries apply CSS conditionally. Mobile-first starts with small-screen base styles and uses `min-width` to enhance for larger screens.

---

### 📌 Q100 — How would you debug a CSS layout bug where an element is not appearing where you expect?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Systematic debugging:

1. Inspect computed styles/box model in DevTools.
2. Check for `display: none`, `opacity: 0`.
3. Check layout context (flex/grid/absolute).
4. Check sizing, padding, borders.
5. Check containing block for absolute positioning.
6. Check cascade/specificity/layers.
7. Check for `overflow` clipping.
8. Check media queries.
   Fix the root cause, don't just add random CSS.

---

---

# 🏗️ HTML Deep Dive & Accessibility

### 📌 Q1 — What is HTML?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
HyperText Markup Language. Structures web content using elements. Not a programming language (no logic/loops). HTML = Structure, CSS = Presentation, JS = Behavior.

---

### 📌 Q2 — What is an HTML element?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Complete unit: opening tag + content + closing tag (e.g., `<p>Hello</p>`). Void elements (like `<img>`, `<input>`) have no closing tag.

---

### 📌 Q3 — What is the difference between an HTML tag and an HTML element?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**  
**Tag**: the markup syntax (`<p>`).
**Element**: the complete structure (`<p>Hello</p>`).

---

### 📌 Q4 — What is the basic structure of an HTML document?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>My Page</title>
  </head>
  <body>
    <h1>Hello</h1>
  </body>
</html>
```

`<head>` = metadata/resources. `<body>` = visible content.

---

### 📌 Q5 — Why is the `lang` attribute important?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Specifies document language. Helps browsers, search engines, translation tools, and screen readers. Can be changed for specific elements.

---

### 📌 Q6 — What are void elements in HTML?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
Elements that cannot have children and don't use closing tags (e.g., `<img>`, `<input>`, `<br>`, `<hr>`, `<meta>`, `<link>`).

---

### 📌 Q7 — What is the difference between HTML entities and normal characters?

> **📊 Difficulty:** 🟡 Medium

> **🕵️ What interviewer expects:** HTML parsing basics.

**💡 Ideal Answer:**
Entities represent special characters (e.g., `&lt;`, `&gt;`, `&amp;`, `&nbsp;`). Prevents the browser from interpreting them as markup.

**🔗 Follow-up:**
_Why can't we simply write `<` inside normal text?_
**↳ Answer:** Because `<` is interpreted as the beginning of a tag.

---

### 📌 Q8 — What is the difference between absolute and relative URLs in HTML?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**

- **Absolute**: complete address (`https://example.com/about`).
- **Relative**: resolved relative to current document (`/about` or `../images/photo.jpg`).

---

### 📌 Q9 — What are the different types of `<input>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**
`text`, `email`, `password`, `number`, `tel`, `url`, `search`, `date`, `checkbox`, `radio`, `file`, `hidden`, `submit`, etc. Using the right type provides semantics, built-in validation, and mobile keyboard optimizations.

---

### 📌 Q10 — What is the difference between `<table>`, `<thead>`, `<tbody>`, `<tfoot>`, and `<tr>`?

> **📊 Difficulty:** 🟢 Easy → 🟡 Medium

**💡 Ideal Answer:**

- `<table>`: entire table.
- `<thead>`: header section.
- `<tbody>`: main data.
- `<tfoot>`: footer/summary.
- `<tr>`: table row.
- `<th>`: header cell. `<td>`: data cell.

---

### 📌 Q11 — How do you make an HTML table accessible?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Use proper semantics: `<caption>` for title, `<th>` for headers, `scope="col"` or `scope="row"` to associate headers with cells. Never use tables for visual layout.

---

### 📌 Q12 — What is the purpose of `<meta charset="UTF-8">`?

> **📊 Difficulty:** 🟢 Easy

**💡 Ideal Answer:**
Specifies character encoding. UTF-8 supports a vast range of characters (including Arabic) and is the modern standard. Prevents corrupted text.

---

### 📌 Q13 — What is the purpose of `<meta name="description">`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Provides a page summary. Search engines may use it as the snippet in search results, improving click-through rates. Not a direct ranking factor.

---

### 📌 Q14 — What is the purpose of `meta name="robots"`?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Instructions for search engine crawlers. `noindex` prevents indexing. `nofollow` prevents crawling links. Does not prevent user access (not an auth mechanism).

---

### 📌 Q15 — What is a canonical URL?

> **📊 Difficulty:** 🟡 Medium → 🔴 Hard

**💡 Ideal Answer:**
Tells search engines the preferred URL when multiple URLs have similar content (`<link rel="canonical" href="...">`). Consolidates SEO signals. Not a redirect.

---

### 📌 Q16 — What is the purpose of `rel` on an HTML link?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Describes the relationship between the document and the linked resource (e.g., `stylesheet`, `canonical`, `noopener`, `noreferrer`).

---

### 📌 Q17 — What is the purpose of `target="_blank"`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**
Opens the link in a new tab/window. Should be paired with `rel="noopener noreferrer"` for security.

---

### 📌 Q18 — What is the difference between `noopener` and `noreferrer`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `noopener`: prevents the new page from accessing `window.opener` (prevents reverse-tabnabbing).
- `noreferrer`: does the above, AND prevents sending the `Referer` HTTP header.

---

### 📌 Q19 — What is the purpose of heading elements `<h1>` through `<h6>`?

> **📊 Difficulty:** 🟡 Medium

> **🕵️ What interviewer expects:** Document structure + accessibility.

**💡 Ideal Answer:**
Represent document outline/hierarchy. Crucial for screen reader navigation. Should reflect logical content structure.

---

### 📌 Q20 — What is the difference between semantic HTML and ARIA?

> **📊 Difficulty:** 🟠 Medium → Hard

**💡 Ideal Answer:**  
Semantic HTML uses native elements with built-in meaning/behavior (`<button>`). ARIA adds accessibility semantics when native elements aren't enough (`role="button"`). **Rule of thumb:** Prefer native HTML first.

---

### 📌 Q21 — What is `tabindex`?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**
Controls keyboard focus. `0` adds to natural tab order. `-1` allows programmatic focus but removes from tab order. Positive values (e.g., `5`) are discouraged.

---

### 📌 Q22 — What is an accessible name?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
The name assistive technologies use to identify an element to the user (e.g., visible text in a `<button>`, or `<label>` for an input). Crucial for screen readers.

---

### 📌 Q23 — Why should you prefer native HTML controls over custom controls?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Native controls (`<button>`) provide semantics, keyboard interaction, focus behavior, and AT support out-of-the-box. Custom `<div>` controls require manual implementation of all these features.

---

### 📌 Q24 — What is the difference between `aria-hidden="true"` and removing an element from the DOM?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
`aria-hidden="true"` hides from the accessibility tree, but the element remains in the DOM (visible to CSS/JS). Removing from DOM deletes it entirely. Never put `aria-hidden="true"` on a focusable element.

---

### 📌 Q25 — What is the difference between `hidden`, `aria-hidden`, and CSS hiding?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

- `hidden`: HTML semantic state, not rendered.
- `aria-hidden="true"`: hidden from AT, but visually present.
- CSS `display: none`: removed from rendering/layout.
- CSS `visibility: hidden`: visually hidden, keeps layout space.

---

### 📌 Q26 — What is the difference between `hidden` and `display: none`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
`hidden` is an HTML state/meaning. `display: none` is a CSS presentation rule. Browsers default `hidden` to `display: none`, but CSS can override it (which can cause accessibility mismatches).

---

### 📌 Q27 — What is the purpose of `<details>` and `<summary>`?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
`<details>` creates a native disclosure widget (accordion). `<summary>` is the clickable label. Provides open/close behavior without JS.

---

### 📌 Q28 — What is the purpose of the `<dialog>` element?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**  
Represents a modal or non-modal dialog. `showModal()` opens it as a modal (blocks background interaction, adds top layer). `close()` closes it.

---

### 📌 Q29 — What is the `<datalist>` element?

> **📊 Difficulty:** 🟡 Medium

**💡 Ideal Answer:**  
Provides a list of suggested values for an `<input>`. Unlike `<select>`, the user can still type a custom value.

---

### 📌 Q30 — What is the purpose of the `<output>` element?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**  
Represents the result of a calculation or user action. Semantically different from `<input>`.

---

### 📌 Q31 — What is the difference between `<progress>` and `<meter>`?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**

- `<progress>`: completion progress of a task (e.g., file upload).
- `<meter>`: scalar measurement within a known range (e.g., disk usage).

---

### 📌 Q32 — What is the purpose of `<noscript>`?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**  
Provides fallback content when scripting is disabled or unsupported. Not a general JS error handler.

---

### 📌 Q33 — What is the purpose of the `<base>` element?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
Specifies the base URL for resolving relative URLs in the document. Only one `<base>` allowed per document.

---

### 📌 Q34 — What is the Constraint Validation API?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
JS API to inspect/control form validity. Uses `validity` object (`valueMissing`, `typeMismatch`, etc.), `checkValidity()`, `reportValidity()`, and `setCustomValidity()`.

---

### 📌 Q35 — What happens when the browser receives an HTML document?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
HTML bytes → Decode → Parse HTML → DOM → Parse CSS → CSSOM → Render Tree → Layout → Paint → Compositing. Browsers can progressively render.

---

### 📌 Q36 — What is `referrerpolicy`?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**  
Controls what `Referer` header is sent with requests. Policies include `no-referrer`, `origin`, `strict-origin-when-cross-origin`. Does not hide IP address.

---

### 📌 Q37 — You need to open an external link in a new tab. How would you write it safely?

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer">Open</a>
```

Prevents reverse-tabnabbing and controls referrer info.

---

### 📌 Q38 — You have this HTML. What's wrong with it?

```html
<p>
  <h2>Available Jobs</h2>
  <div>Frontend Developer</div>
</p>
```

> **📊 Difficulty:** 🔴 Hard

**💡 Ideal Answer:**
Invalid nesting. `<p>` can only contain phrasing content. `<h2>` and `<div>` are flow content. The browser will auto-close the `<p>` tag. Restructure using `<section>` or `<article>`.

---

### 📌 Q39 — What is the difference between `inputmode` and `type` on an input?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**

- **`type`**: controls semantics and validation (e.g., `type="email"` validates email).
- **`inputmode`**: hints the mobile virtual keyboard layout (e.g., `inputmode="numeric"` shows digits). Does not change validation.

**🔗 Follow-up:**
_Does `inputmode` affect desktop behavior?_
**↳ Answer:** No. It's strictly for mobile virtual keyboards. Validation still relies on `type`, `pattern`, etc.

---

### 📌 Q40 — What does `pointer-events: none` do, and how is it different from `visibility: hidden`?

> **📊 Difficulty:** 🟠 Medium

**💡 Ideal Answer:**

- **`pointer-events: none`**: Element is visible and in layout, but ignores mouse/touch clicks. **Crucial:** It does NOT prevent keyboard focus or screen reader access.
- **`visibility: hidden`**: Element is invisible, keeps layout space, and is removed from the accessibility tree.

**🔗 Follow-up:**
_Can a keyboard user still interact with an element that has `pointer-events: none`?_
**↳ Answer:** Yes! `pointer-events: none` only disables mouse/touch. To properly disable, use the `disabled` attribute, or `aria-disabled="true"` with JS event blocking.
