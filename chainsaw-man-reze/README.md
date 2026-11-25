# Chainsaw Man Reze

Theme for claude-ui. Fan-made, personal use. Characters and artwork belong to their owners.

- Blurred art background in light and dark, panels frosted over it, matching colours.
- Dancing-figure loader, rotating "Thinking" text, burning bomb while running, exploded bomb after a tick.
- Capabilities: none.

Needs Claude UI 1.5 or newer (`claudeUi: ">=1.5"`).

Images are files in `images/`, declared as `assets` in `addon.json`:

| File | Used as |
| --- | --- |
| `bg-light.jpg`, `bg-dark.jpg` | Theme `background` per mode (veil 0.26, dark 0.42; panel alpha 0.56) |
| `dance.webp` | `loader` slot: sidebar and tab spinner |
| `boom.svg` | `done-icon` slot: finished tool call |
| `bomb.svg` | Running tool call, from `theme.css` |

A missing file is allowed: without a background file the panels stay opaque; without a slot file the built-in mark shows. The rotating Thinking text is CSS; the `thinking-phrases` slot holds the same words and shows when reduced motion is on.

Install: `/addons` > Local folder > this folder path > Approve and enable. Settings > Appearance > pick "Chainsaw Man Reze". `theme.css` applies only while this theme is picked.
