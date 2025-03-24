# ShyGnomeFox changes

This file documents all of the changes made by ShyGnomeFox to the Firefox GNOME theme,
since I don't feel like using a git submodule or whatever for it.

- All mentions of `../icons/` have been changed to `icons/`.
- `popups.css:202`: `background` was changed to `background-color` to fix a grid of icons
  appearing on hover of context menu entries when using `shyfox.enable.context.menu.icons`.
- TODO: `findbar.css` is probably desirable to have, but requires fixes (the find bar's checkboxes go
  partially under the search box, the find bar's previous/next buttons partially overlap the search box).
- TODO: `entries.css` is probably desirable to have, but requires fixes (the URL bar's results background is transparent).
- TODO: `controls.css` is probably desirable to have, but may require fixes (checked checkboxes are difficult to see on dark themes).
- FIXME: `buttons.css` and `buttons-fixes.css` break the width of the application menu button and the extensions button.
- FIXME: `buttons.css` and `buttons-fixes.css` make the find bar's previous/next buttons overlap with each other.
- FIXME: `buttons.css` and `buttons-fixes.css` make the back/forward/refresh buttons in the URL bar lose their top margins.
