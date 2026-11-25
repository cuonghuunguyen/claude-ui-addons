# Neon City

Theme for claude-ui. Cyberpunk HUD: navy-black (dark) / pale blue-white (light) surfaces, cyan primary, magenta keywords. Cut-corner glass panels over city pictures, rain, tab glitch, HUD loaders, rotating conic border on the focused prompt box. Capabilities: none.

Background: dark = street picture cross-fading with a tower picture, light = a sunlit city picture. Files in `images/` (`street.webp`, `tower.jpg`, `day.jpg`; rain layers `rain1-2.svg`).

Needs Claude UI 1.5 or newer (`claudeUi: ">=1.5"`). `theme.css` is the theme CSS (`themes[].css`): it applies only while Neon City is picked. Selectors use stable `data-part` names where the app has a part.

Install: `/addons` > Local folder > path of this folder > Approve and enable. Then Settings > Appearance > Neon City. Theme options: Rain (default on), Light rain.

Pictures belong to their owners. Personal use only; removed on request.

Layer variables (CSS custom properties on `:root[data-theme="addon:neon-city:neon"]`, zero specificity): `--neon-veil`, `--neon-glass`.
