# 📦 Module 3: The Box Model Log

### 🗓 Day 11: July 1, 2026
- **Topics:** Introduction to the Box Model & Box Model Essentials
- **Log:** 
  - **Box Concept:** Conceptualized all HTML nodes as rectangular boxes divided into two core behaviors: **Block elements** (starts a new line, fills container width) and **Inline elements** (flows within text content, vertical margins/paddings do not impact layout flow).
  - **The Four Layers:** Analyzed the structural anatomy of the Box Model: **Content** (inner core), **Padding** (internal space breathing room), **Border** (outer edge boundary), and **Margin** (external clear space between neighboring boxes).
  - **Dimension Formulas:** Practiced tracking how the browser computes overall box sizes by default. 
    - $\text{Total Width} = \text{Width} + \text{Left/Right Padding} + \text{Left/Right Border} + \text{Left/Right Margin}$
    - $\text{Total Height} = \text{Height} + \text{Top/Bottom Padding} + \text{Top/Bottom Border} + \text{Top/Bottom Margin}$
  - **Sizing Constraints:** Evaluated box boundaries using min/max limits (`min-width`, `max-width`, `min-height`, `max-height`).
  - **Style Configurations:** Tested directional longhands against multi-value shorthand properties for paddings and margins. Reviewed border styles (`solid`, `dashed`, `double`, `inset`).
- **Key Takeaway:** Setting `width` or `height` on an element only alters its internal content box by default; any added padding or borders scale the element's actual footprint outward on the screen.