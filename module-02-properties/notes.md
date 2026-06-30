# 📦 Module 2: CSS Properties & Values Log

### 🗓 Day 6: June 24, 2026
- **Topics:** Colors, Color Models, and Color-Related Properties
- **Log:** 
  - **Color Models:** Reviewed **RGB/RGBA**, **HEX**, and **HSL/HSLA**. Noted that RGB is native to digital displays, while HSL is highly intuitive for manual tweaking. Explored alternative systems like **CMYK** (printing) and **HSV** (shades/tints), alongside browser quirks with predefined color names (e.g., `green` vs `lime`).
  - **Core Properties:** Practiced using `color` for typography and `background-color` to control the visual plane behind text content.
  - **Shorthands & Layout:** Tested composite shorthand properties like `background` and `border` (which bundles width, style, and color together). Note: `border-color` requires a defined `border-style` to render.
  - **UI Enhancements:** Explored properties that rely on color values for depth and interactive feedback, including `box-shadow` (using RGBA for smooth alpha transparency), `outline-color` (for input fields in a `:focus` state), `text-shadow`, and `caret-color` (typing cursor).
- **Key Takeaway:** Color properties control hierarchy and user interaction states; using alpha transparency (`rgba`) for UI elements like shadows creates a cleaner, more realistic visual depth than solid colors.

### 🗓 Day 7: June 26, 2026
- **Topics:** Weekly Review & Portfolio Project Review Day (Weekly Build)
- **Log:** - **Weekly Consolidation:** Reviewed all concepts covered from Day 1 to Day 6, verifying understanding of selectors, specificity, inheritance, and the cascade hierarchy.
  - **Portfolio Application:** Applied Module 1 and Module 2 principles to the independent personal portfolio landing page repository.
  - **Review Scope:** Verified design system integration using custom properties for the brand color palette (deep blue, mustard gold, and light gray-white) and tested alpha-transparent `box-shadow` values on UI components.
- **Key Takeaway:** Building weekly ensures that abstract concepts like specificity overrides and color models transition immediately from theory into scalable, real-world project architecture.

### 🗓 Day 8: June 28, 2026
- **Topics:** Background Properties, Gradient Functions, Shorthand vs. Longhand Properties
- **Log:** 
  - **Background Control:** Mastered `background-image` alongside positioning modifiers: `background-repeat` (`repeat`, `x/y`, `no-repeat`) and `background-size` (comparing `cover` to crop/fill vs `contain` to preserve ratio).
  - **Visual Dynamics:** Discovered `background-blend-mode: overlay` to blend base colors with background images, and `background-attachment: fixed` to create stationary background scrolling effects.
  - **CSS Gradients:** Practiced writing color functions directly inside `background-image`: `linear-gradient(to bottom, #ff9900, #ffcc00)` and `radial-gradient(circle, #ff9900, #ffcc00)`.
  - **Shorthand Optimization:** Compared verbose longhand rules against single-line shorthand declarations. Mastered the background shorthand syntax matrix: `background: [image] [position] / [size] [repeat] [color]`.
- **Key Takeaway:** Gradients are treated as images by the browser. When writing background shorthand properties, the background size *must* explicitly follow the position, separated by a forward slash (e.g., `top right / cover`).

### 🗓 Day 9: June 29, 2026
- **Topics:** CSS Text Styling Properties & List Properties
- **Log:** 
  - **Font Mechanics:** Explored text hierarchy using `font-family` stacks (ending with web-safe fallbacks like `sans-serif` or `monospace`), `font-weight` (normal/bold or numerical scales $100-900$), and `font-style` variations.
  - **Sizing Units:** Evaluated font sizing strategies, noting the precision of absolute units (`px`) versus the scalability of relative units: `em` (relative to parent element size) and `rem` (relative to the root `<html>` element).
  - **Text Manipulation:** Practiced text formatting layouts with alignment options (`text-align: justify`), case conversions (`text-transform`), spacing rules (`letter-spacing`, `word-spacing`), vertical breathing room (`line-height: 1.6`), and decorative accents like underlines (`text-decoration`) or `text-shadow`.
  - **List Customization:** Studied `<ol>` and `<ul>` semantic modifications. Used `list-style-type` (e.g., `circle`, `lower-roman`) and `list-style-image`. 
  - **Marker Alignment:** Tested `list-style-position` behaviors, analyzing how `inside` places the bullet within the flow of content while `outside` projects it outside the element container box.
  - **Layout Spacing:** Experimented with layout cleaning by stripping default list padding (`padding-left: 0`) and customizing individual list items (`li`) using custom borders, background colors, internal padding, and external block spacing (`margin-bottom`).
- **Key Takeaway:** `rem` is preferred over `em` for font scaling in complex applications because it evaluates predictably against the root font size rather than compounding through nested elements. For layout styling, stripping browser-default list margins and paddings provides full structural control over component design.

### 🗓 Day 10: June 30, 2026
- **Topics:** Hyperlink States, Image Presentation Properties, & Module 2 Completion
- **Log:** 
  - **Hyperlink Pseudo-classes:** Mastered the **LVFHA** specific order principle (`:link`, `:visited`, `:focus`, `:hover`, `:active`) to ensure correct browser cascade rules when overriding core link aesthetics.
  - **Asset Scaling:** Studied visual media container rules, using `max-width: 100%` for basic fluid responsiveness alongside `object-fit: cover` to cleanly resize imagery while preserving natural aspect ratios. 
  - **Aesthetic Refinement:** Explored decorative layout enhancements using `border-radius` variants (including specific directional shorthand values and `50%` configurations for circular crops) and transparency shadows.
  - **Direct Manipulation:** Tested the native `filter` function properties to alter image bitmaps natively inside the browser container engine (such as `grayscale()`, `blur()`, and `brightness()`).
  - **Layer Depth:** Examined the `z-index` property matrix to explicitly control stacking orders on overlapping absolute-positioned structural components.
- **Key Takeaway:** The exact ordering of link pseudo-classes (LVFHA) is a mandatory architectural design rule; reversing them breaks the CSS cascade. Similarly, combining absolute sizing bounds with `object-fit: cover` keeps images crisp and contained without distortion.