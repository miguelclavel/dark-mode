# Dark Mode

A dark mode that remembers you, from [miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=dark-mode).

<img src="assets/demo.gif" width="720" alt="A dark mode that remembers you: a screen recording">

**[Try it live](https://miguelclavel.github.io/dark-mode/)** · one file, `index.html`, no libraries, no build step.

If your site forgets dark mode the moment someone refreshes the page, that's not a design choice. That's a bug.

Mine has a small toggle in the corner. Click it and the whole site switches between light and dark. Come back tomorrow, and it's still exactly how you left it.

The part people usually skip: on someone's very first visit, before they've touched the toggle at all, the site checks their operating system's own dark mode setting and matches it. Nobody has to make a choice they didn't already make once, in their system settings.

Here's the prompt:

Try switching it a couple times. I still think it's more fun than a toggle has any right to be.

## Use it on your site

Three pieces, all in `index.html`: the tiny script in the `<head>` (it runs before the page paints, which is what stops the flash of the wrong theme), the two sets of colour variables (`:root` and `:root[data-theme="dark"]`), and the button with its script. The choice is saved under the `theme` key. Until someone picks, the page keeps following the system setting, even if it changes while they're reading.

## Or build your own from the prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Add a button that switches the whole site between a light and dark color theme. When the visitor picks one, save their choice in localStorage so it's remembered the next time they visit. On their very first visit, before they've chosen anything, check their operating system's dark mode setting and match the site to it instead of defaulting to light.
```

More like this in [interaction-recipes](https://github.com/miguelclavel/interaction-recipes).

---

MIT licensed. Made by [Miguel Clavel](https://miguelclavel.com/?utm_source=github&utm_medium=dark-mode) with Claude Code. If you build one of these, send it to me. I'd genuinely like to see it.
