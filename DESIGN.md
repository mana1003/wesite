# Design system: Manali Jain portfolio (Taravi brand)

Palette and logo shape come from the Taravi pitch deck. Direction is from the brief, not from real-site comparisons (UXKIN tools were not connected).

## Color (dark only)
| Token | Value | Role |
|---|---|---|
| --bg | #0f1222 | page, deep navy |
| --surface | #171b30 | tiles |
| --panel | rgba(20,24,41,.8) | text panels over the 3D background |
| --ink | #f4f1ea | text |
| --mute | #aeb1c8 | secondary text |
| --line | rgba(255,255,255,.13) | borders |
| --gold | #e0ac4f | primary: buttons, links, nodes, highlights |
| --violet | #8f86e0 | accent: small stars, tags |
| --ok | #5fd08a | verified states |

## Typography
Apple system stack (-apple-system, SF Pro Display/Text), then Segoe UI, Roboto, Arial. Weights 400, 600, 700. Display tracking -0.035em. Body 17px.

## Spacing and shape
8px base. Content width 1080px. Radius 12 / 20 / 28. Section padding 96px.

## 3D background
Three.js: ~1,100 twinkling stars the camera flies through as you scroll, plus 12 gold nodes that morph by section: Taravi constellation (hero, contact), birth-chart wheel (Taravi, projects), rover path (autonomy). Nodes glow near the cursor; the scene tilts with the mouse; click empty space for a pulse.

## LiDAR drive (after Taravi)
Interactive Three.js scene in its own rounded viewport: LiDAR point-cloud terrain, a wireframe car with a sweeping scan ring, and simulated obstacles that turn gold in range and violet once mapped. Drag to orbit, scrub the slider to drive, toggle Detections and Top view. It only renders while on screen. Labelled "Simulated scene".

## Content rules
No pitch-deck metrics (user counts, conversion, cost per answer, market size, fundraising) anywhere on the site.

## Motion
GSAP + ScrollTrigger: one hero entrance and section reveals. Header shows scroll progress; nav highlights the current section. Tiles: cursor tilt, spotlight, flip, and a per-tile animation driven by cursor position. Reduced motion: static scene, no entrances.
