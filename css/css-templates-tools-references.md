# CSS
## Boilerplate HTML & CSS Templates
* Review the html and css folders in this repo.
* Review/use the [forked html5 boilerplate repo] (<https://github.com/onesojourner/fork-html5-boilerplate/tree/branch>) for both an HTML5 and CSS templates.
* [Pico CSS] (<https://https://picocss.com>): A minimalist and lightweight starter kit that prioritizes semantic HTML. It makes every HTML element responsive and elegant by default.
* [Simple CSS] (<https://simplecss.org/>): A classless framework that styles semantic HTML to look good quickly. It's designed for use with plain HTML and requires no classes for a great-looking site.
* [Pure CSS] (<https://pure-css.github.io/>): Developed by Yahoo, Pure is a set of small, responsive CSS modules that can be used as a lightweight foundation. Its design is unopinionated, making it easy to customize with your own CSS rules.
* [Skeleton CSS] (<http://getskeleton.com/>):  A dead simple, responsive boilerplate that is extremely minimal, focusing on a basic grid and styling for core elements. 
* [Tailwind CSS] (<https://tailwindcss.com/>): A utility-first framework that provides low-level utility classes like flex, pt-4, and text-center that can be composed to build any design, directly in your HTML. It is a very popular choice for modern web development. Offers pre-defined classes or components for building interfaces, providing more comprehensive control over the design. 
---
## Modern CSS Reset (Boilerplate Logic)
* Modern foundation: A typical 2026 boilerplate should include:
  * Box Model Reset: Use box-sizing: border-box on all elements.
  * Image Fluidity: Force images to behave with max-width: 100% and display: block.
  * Smooth Scrolling: Enable scroll-behavior: smooth for better user experience.
  * System Fonts: Use native system font stacks for better performance and a "native" feel

## CSS Reset
1. Modern resets, like the one by Josh Comeau or the modern-normalize library, go beyond traditional resets by incorporating modern best practices
~~~
/* A Modern CSS Reset (example snippets) */

*, *::before, *::after {
  box-sizing: border-box; /* Ensures padding and border are included in the element's total width/height */
}

body {
  margin: 0; /* Remove default body margin */
  line-height: 1.5; /* Improves readability */
  -webkit-text-size-adjust: 100%; /* Prevents text zooming on iOS devices */
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; /* Use modern system fonts */
}

img, picture, video, canvas, svg {
  display: block;
  max-width: 100%; /* Force images/media to behave responsively */
}

input, button, textarea, select {
  font: inherit; /* Ensures form elements inherit the body's font styles */
}

p, h1, h2, h3, h4, h5, h6 {
  overflow-wrap: break-word; /* Prevents long words from breaking the layout */
  margin-top: 0; /* Control margin with utility classes or components */
}

/* Remove list styles (optional, based on preference) */
ul, ol {
  list-style: none;
  padding: 0;
  margin: 0;
}

/* Add an opinionated default for interactive elements */
a {
  text-decoration: none;
  color: inherit;
}
~~~
2. Base Styles and Quality-of-Life Tweaks
These styles set up initial variables and useful defaults that can be easily overridden.
 
* CSS Custom Properties (Variables): Define common colors, font sizes, and spacing at the :root level for consistency.
~~~
:root {
  --primary-color: #007bff;
  --text-color: #333;
  --bg-color: #fff;
  --spacing-sm: 0.5rem;
  --spacing-md: 1rem;
}
~~~
* Smooth Scrolling (Optional): A user-requested feature for single-page applications
~~~
html {
  scroll-behavior: smooth; /* Enables smooth scrolling when using anchor links */
}
~~~
* Focus Management: Ensure keyboard users have clear focus indicators.
~~~
a:focus, button:focus, input:focus {
  outline: 2px solid var(--primary-color);
  outline-offset: 3px;
}
~~~
---
## CSS Reset v2
2026 CSS reset is composed of several critical functional blocks. These components transition your CSS from a "reactive" state (fixing browser bugs) to a "proactive" state (setting modern design defaults).

**1. Box Model Component**

* **Property:** box-sizing: border-box

* **The Function:** This is the most essential rule. By default, the CSS box model adds padding and borders outside the defined width of an element. This reset forces them inside, making layout math much more intuitive.

* **Application:** Usually applied to *, *::before, and *::after to ensure every element on the page behaves predictably. 

**2. Typographic & Legibility Foundations**
Modern resets prioritize readability and accessible defaults rather than just stripping styles.

* **Accessible Line Height:** Setting line-height: 1.5 on the body or :root ensures text is legible and meets WCAG accessibility standards.

* **Text Smoothing:** Using -webkit-font-smoothing: antialiased renders text more clearly on macOS and iOS devices.

* **Advanced Text Wrapping:** Using text-wrap: balance for headings prevents "orphaned" words (single words on a new line), while text-wrap: pretty for paragraphs improves the overall typographic flow. 

**3. Form Element Inheritance**

* **The Problem:** Historically, elements like <input>, <button>, and <textarea> do not inherit the font or size from their parent elements.

* **The Fix:** Adding font: inherit ensures these elements automatically match your site's typography without needing manual 
styling. 

**4. Fluid Media Defaults**

* **Property:** max-width: 100% and display: block

* **The Function:** These rules prevent large images, videos, or SVGs from overflowing their containers and breaking the mobile layout. Setting them to block also removes the small unwanted gap often found at the bottom of inline images. 

**5. Animation & Motion Control**

* **Keyword Interpolation:** New for 2025–2026, interpolate-size: allow-keywords enables smooth CSS transitions for values like: 
  * height: auto, which previously required JavaScript.

* **Motion Sensitivity:** Resets now include a prefers-reduced-motion media query to instantly stop all animations for users who have motion sensitivities. 

**6. Layout Hygiene**

* **Stacking Context Isolation:** Applying isolation:isolate to root containers (like #root or #__next) prevents unexpected z-index issues where background elements might overlap with modals or navbars.

* **Scroll Management:** Setting scroll-behavior: smooth (only when motion is preferred) provides a better user experience for anchor links.

* **Margin Resets:** Stripping margins from common elements like h1, h2, p, and figure allows you to control spacing strictly through your own design system rather than fighting browser defaults.

---
## Tools 
* [CSS Analytics] (https://www.projectwallace.com/)
* [CSS Specificty Vizualizer] (https://isellsoap.github.io/specificity-visualizer/)
* [HTML & CSS Online Interactive] (https://html-css-js.com/css/)
* [Specicicity Calculator] (https://polypane.app/css-specificity-calculator/)

## Guides
5 [cas-tricks Guides] (https://css-tricks.com/guides/)

## Key References

