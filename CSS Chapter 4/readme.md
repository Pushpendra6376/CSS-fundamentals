in this chapter we  are learning about css units : absolute , realtive,CSS float layout and css Positions 


firstly we are learning about css units 
there are two types of it 
1. absolute
2. relative

# 📏 CSS Units Summary

CSS uses different types of **units** to define dimensions like width, height, margin, padding, font-size, etc.

---

## 📌 1. **Absolute Units**
These units are fixed and do not scale with screen size.

| Unit | Meaning        | Example      |
|------|----------------|--------------|
| px   | Pixels         | `width: 100px;` |
| cm   | Centimeters    | `width: 5cm;`   |
| mm   | Millimeters    | `width: 10mm;`  |
| in   | Inches         | `width: 1in;`   |
| pt   | Points (1/72 in) | `font-size: 12pt;` |
| pc   | Picas (1/6 in) | `font-size: 1pc;`  |

📝 *Use mainly `px` for screen designs.*

---

## 📌 2. **Relative Units**
These scale based on parent size or screen.

| Unit  | Relative To                         | Example              |
|-------|-------------------------------------|----------------------|
| %     | Parent element                      | `width: 50%;`        |
| em    | Font size of the element's parent   | `padding: 2em;`      |
| rem   | Font size of the root element       | `font-size: 1.5rem;` |
| vw    | 1% of the viewport width            | `width: 100vw;`      |
| vh    | 1% of the viewport height           | `height: 100vh;`     |
| vmin  | Smaller of `vw` or `vh`             | `font-size: 3vmin;`  |
| vmax  | Larger of `vw` or `vh`              | `font-size: 3vmax;`  |
| ex    | x-height of current font            | `line-height: 2ex;`  |
| ch    | Width of the "0" character          | `width: 20ch;`       |

📝 *Use `rem` for consistent typography, `vw/vh` for responsive layouts.*

---

## 🔖 Tips

- Prefer `rem` over `em` for consistent scaling.
- Use `vw`/`vh` for full-screen or responsive components.
- Avoid mixing too many unit types in the same layout.
- `%` is great for fluid, parent-relative designs.

---

✅ Choose units based on context:  
Use `px` for precision, `rem/em` for typography, `%` for layout, and `vw/vh` for responsiveness.

















credits :- A youtube channel name harsiht vasishta 
link :- https://www.youtube.com/watch?v=odAwZLHHCgQ&list=PLwgFb6VsUj_mtXvKDupqdWB2JBiek8YPB&index=72