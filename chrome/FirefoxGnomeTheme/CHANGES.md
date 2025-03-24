# ShyGnomeFox changes

This file documents all of the changes made by ShyGnomeFox to the Firefox GNOME theme,
since I don't feel like using a git submodule or whatever for it.

- All mentions of `../icons/` have been changed to `icons/`.
- `popups.css:202`: `background` was changed to `background-color` to fix a grid of icons
  appearing on hover of context menu entries when using `shyfox.enable.context.menu.icons`.
- `buttons.css:92-133`: Removed entire CSS block, which made the `toolbarbutton` element
  change color on hover. See the below change for motivation.
- `buttons-fixes.css:16-21`: Removed entire CSS block, which made the `image` child of
  `toolbarbutton` not change color on hover.
  - The reason for removing these is that for the toolbar buttons (e.g. back/forward/refresh),
    having these blocks "shifts" the "responsibility" of changing color on hover from the
    `image` child element `toolbarbutton` to the `toolbarbutton` itself, which has a different
    size, which (undesirably) changes the size and thus shape of the hover effect.
- TODO: `findbar.css` is probably desirable to have, but requires fixes (the find bar's checkboxes go
  partially under the search box, the find bar's previous/next buttons partially overlap the search box).
- TODO: `entries.css` is probably desirable to have, but requires fixes (the URL bar's results background is transparent).
- TODO: `controls.css` is probably desirable to have, but may require fixes (checked checkboxes are difficult to see on dark themes).
- FIXME: `buttons.css` and `buttons-fixes.css` break the width of the application menu button and the extensions button.
- FIXME: `buttons.css` and `buttons-fixes.css` make the find bar's previous/next buttons overlap with each other.
