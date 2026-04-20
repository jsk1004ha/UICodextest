# Cosmic Beauty

A production-ready, single-file cinematic landing experience that presents a calm, hyper-realistic cosmic environment.

## Overview

`index.html` contains the entire experience (structure, style, animation, and interaction) in one deployable file.

The page emphasizes:

- immersive deep-space atmosphere
- minimal poetic typography
- subtle, slow environmental motion
- enhanced first-viewport readability with brighter hero glow and stronger copy contrast
- progressive enhancement for performance
- accessibility-conscious interaction and readability

## Run locally

You can open the file directly in any modern browser:

```bash
open index.html
```

Or serve it from a local static server:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Interaction model

- Primary CTA: **Explore the Cosmos**
- Secondary CTA: **View Celestial Wonders**
- Scroll behavior introduces gentle depth and parallax shifts
- CTA hover uses soft glow and subtle scale only

## Performance and compatibility

- Uses a lightweight `canvas` starfield with capped DPR for efficiency
- Reduces star density and motion on lower-power/mobile contexts
- Pauses animation when tab visibility is hidden
- Respects `prefers-reduced-motion`

## Accessibility notes

- Semantic sectioning (`main`, `section`, `nav`)
- High contrast foreground typography over layered dark background
- Visible keyboard focus via button hover/focus styling
- Motion reduction behavior for users with reduced-motion preferences
