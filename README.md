# claude-ui-addons

Addons for [claude-ui](https://github.com/cuonghuunguyen/claude-code-ui). An addon changes the claude-ui web app: color themes, panes, bands, slash commands, code fence and tool renderers. Full addon reference: [addons.md](https://github.com/cuonghuunguyen/claude-code-ui/blob/main/docs/site/features/addons.md).

## Addons

| Folder | Type | Capabilities | Description |
| --- | --- | --- | --- |
| [`chainsaw-man-reze`](chainsaw-man-reze) | Theme | none | Chainsaw Man Reze: art background, palettes, dancing loader, bomb animations. Images in `images/`. |
| [`neon-city`](neon-city) | Theme | none | Neon City: cyberpunk HUD glass panels, city pictures as background (slideshow dark, one picture light), rain, glitch, HUD loaders. Images in `images/`. |
| [`gojo`](gojo) | Theme | none | Gojo: manga style, art background (dark and light), Six Eyes eye loader, Unlimited Void intro on opening Focus, Black Flash charge and release, cursed energy smoke, cyan cursed energy aura on prompt focus, animated usage gauge. Images in `images/`. |
| [`liquid-glass`](liquid-glass) | Theme | none | Liquid Glass (Apple iOS 26 style): blurred, saturated glass with specular rims on the prompt box, active tab, menus, dialogs, palette, toasts; transparent title bar (macOS 26); translucent panels; solid content. Own mesh-gradient wallpapers. Refraction (SVG lens) in Chrome and Edge. Options: variant, blur, tint, panel opacity, frosted panels, refraction, reduce transparency. |

## Install

Each addon is one folder with `addon.json` at its root. Needs Claude UI 1.5 or newer. This repo holds many addons, so install from a local clone, not from the repo URL.

1. Clone the repo on the machine that runs claude-ui:
   ```sh
   git clone https://github.com/cuonghuunguyen/claude-ui-addons.git
   ```
2. In claude-ui, enter `/addons` in the prompt box.
3. Choose **Local folder**, enter the absolute path of the addon folder (example: `/path/to/claude-ui-addons/chainsaw-man-reze`), then **Install**.
4. Review the approval card, then **Approve and enable**.
5. For a theme: Settings > Appearance > pick the theme.

Update: `git pull`. claude-ui reads a local folder again each time the dialog opens. A new capability needs a new approval.

## Add an addon

1. Create `<name>/addon.json`. `name`: lowercase letters, digits, `-`, max 64.
2. Declare every capability the addon uses. An addon without capabilities cannot read sessions, send prompts or access the network.
3. Add a `README.md` with install notes and a list of required assets.
4. Do not commit copyrighted assets or secrets.

## License

Fan-made addons reference third-party works. Characters, artwork and pictures belong to their owners. `neon-city` bundles city pictures: personal use, removed on request. `chainsaw-man-reze` bundles fan art (backgrounds, dancing loader) in `images/`: personal use, all rights stay with the owners; it is removed on request. `gojo` bundles fan pictures and a short clip (backgrounds, Unlimited Void, eye) in `images/`: personal use, all rights stay with the owners; removed on request.
