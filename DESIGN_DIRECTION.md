# Aureveil Studio Design Direction

This repo is moving toward a premium editorial wedding invitation style inspired by the Pinterest board reference.

## Visual Direction

- Solid paper objects, not transparent glass.
- Soft sage, ivory, powder blue, charcoal, and warm black.
- Watercolor paper grain and soft natural shadows.
- Embossed or debossed floral artwork.
- Laser-cut or die-cut floral panel edges.
- Minimal serif typography with generous quiet space.
- Handwritten script only as a small accent, not the main style.
- Editorial wedding-film layout language: calm, romantic, premium, restrained.

## Invitation Cover Direction

The final opening cover should feel like a physical stationery piece:

- A solid paper gatefold or wrap cover.
- Left and right floral panels open outward.
- A monogram seal acts as the tap point.
- The inner invitation card rises/slides out after the panels open.
- The animation should feel slow, soft, and tactile.
- Avoid glassmorphism, heavy gradients, generic envelope triangles, or oversized button text.

## Recommended Asset Exports

Design one full cover artboard at:

```text
840 x 1280 px
```

Export transparent PNG assets:

```text
public/assets/envelope-back.png      840 x 1280 px
public/assets/envelope-left.png      460 x 1280 px
public/assets/envelope-right.png     460 x 1280 px
public/assets/seal.png               220 x 220 px
public/assets/invitation-card.png    760 x 1120 px
```

Optional:

```text
public/assets/floral-overlay.png     840 x 1280 px
public/assets/paper-texture.png      840 x 1280 px
```

## Animation Notes

- Left panel: rotate open from the left edge.
- Right panel: rotate open from the right edge.
- Seal: fade and scale down at the start of opening.
- Invitation card: rise after panels begin opening.
- Use easing similar to `cubic-bezier(0.2, 0.76, 0.18, 1)`.

## Current Status

The current site uses CSS/SVG as a prototype. The final production version should replace the CSS panels, floral linework, and seal with exported PNG artwork from Figma for more realistic paper edges, embossing, shadows, and die-cut details.
