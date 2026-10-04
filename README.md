# CSS Box Model Visualizer

A single-page HTML/CSS demo that visually illustrates the **CSS box model**: content, padding, border, and margin. Each layer is shown in its own color and labeled so you can see how they nest.

## Files

| File | Description |
|------|-------------|
| `index.html` | The complete demo (HTML and CSS in one file) |

## What It Shows

| Layer | Color | Value used |
|-------|-------|------------|
| Container (`.con`) | Teal | 80% width, full viewport height |
| Margin area (`.box`) | Sky blue | Space around the blue box, set on `.box1` (`55px 20px 30px 75px`) |
| Border (`.box1`) | Navy | `40px solid navy` |
| Padding (`.box1`) | Blue | `70px 10px 20px 100px` |
| Content (`.box2`) | Orange | Labeled "Context" |

The `Margin`, `Border`, and `Padding` text labels are absolutely positioned on top of the matching regions.

## Getting Started

No installation or build step is needed.

1. Save `index.html` to a folder.
2. Open it in any modern web browser.

## Key Concepts Demonstrated

- `margin`, `border`, and `padding` with different values per side (top, right, bottom, left shorthand)
- `box-sizing: border-box` applied globally with a `*` reset
- Flexbox centering (`display: flex`, `align-items`, `justify-content`)
- `position: absolute` with `top` / `left` percentages for labeling
- Percentage-based sizing and `vh` units

## Known Limitations

- The labels use percentage positions, so they may not line up exactly on all screen sizes.
- Not responsive; best viewed on a desktop browser.
- The label "Context" in the orange box is likely meant to read "Content".
- The page title is the default "Document" and the heading reads "Box ploting" (likely "Box plotting").

## Possible Improvements

- Position the labels relative to their boxes instead of the page, so they stay aligned at any size
- Fix the "Context" and "Box ploting" typos and set a descriptive `<title>`
- Add hover effects or tooltips showing each layer's pixel values
- Add controls (sliders) to change margin, border, and padding live
- Move the CSS into a separate stylesheet
