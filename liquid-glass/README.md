# Liquid Glass

Theme for claude-ui in the style of Apple Liquid Glass (iOS 26 / macOS 26). Needs Claude UI 1.5 or newer. No capabilities. All images are own work (SVG).

## Layers

| Layer | Surfaces | Effect |
| --- | --- | --- |
| Glass | active tab (capsule), prompt box, menus, popovers, select, dialogs, palette, toasts, tooltip, permission and question panels, scroll-to-bottom | blur + saturate + tint, specular rim, shadow; refraction in Chromium |
| Translucent | sidebar, session area, side panel, focus page | see-through fill, edge light, no blur (scroll performance) |
| Transparent | title bar (desktop) | no fill, wallpaper shows through; phones and reduce transparency keep a bar |
| Solid | messages, tool cards, code, diffs, terminal, editor | opaque palette |

## Options (Settings > Appearance)

| Option | Default | Effect |
| --- | --- | --- |
| Glass variant | Regular | Clear: more transparent, dimmed in dark mode |
| Blur (px) | 16 | Blur radius of glass |
| Glass tint | 0.55 | Opacity of the glass fill |
| Panel opacity | 0.62 | Opacity of the translucent panels |
| Blur main panels | off | Blur the large panels too; slower while scrolling |
| Refraction | on | Bent edges (images/lens.svg). Chrome and Edge only; other browsers show blur only |
| Reduce transparency | off | Solid surfaces. Also applied by the OS settings Reduce transparency and Increase contrast |

## Notes

- Menus, popovers and dialogs are selected by role and the `bg-popover` class, not by a stable part. A claude-ui release can break them.
- Phones (below 768 px): glass only on the prompt box and popups, no refraction.
