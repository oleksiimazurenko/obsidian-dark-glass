# Dark Glass

A calm dark theme for [Obsidian](https://obsidian.md): the workspace becomes floating glass cards over an even graphite backdrop, with one warm amber accent.

![Dark Glass: a note with the file explorer and outline](screenshots/workspace.png)

## What it does

- **Glass cards.** The note area and both side docks are rounded, translucent cards with a thin light edge, one gap and one radius everywhere.
- **Graphite backdrop.** An even, colourless gradient behind everything. No coloured glows.
- **Pill tabs.** Tabs are free-standing pills with a gap above the note, never glued to the pane. Stacked tabs stay readable.
- **Frosted layers.** Menus, the command palette, modals, suggestions, hover previews and notices blur what lies beneath them (desktop only).
- **Settings window.** Obsidian 1.15 opens Settings in its own window; it gets the same backdrop, glass navigation and setting cards.
- **Quiet inline fields.** Properties, rename fields and the inline title have no boxes until you hover or focus them.
- **Montserrat** for text and interface, embedded in the theme, and the system monospace font for code.
- **Plugin touches.** The Self-hosted LiveSync status and the Strange New Worlds counter become small pills that do not overlap.

![The command palette in frosted glass](screenshots/command-palette.png)

## Modes

Dark mode only. In light mode Obsidian's default look is used.

On mobile the same palette is drawn with flat fills and no cards or blur, so a phone does not pay for backdrop filters.

## Install

From Obsidian, once the theme is listed in the community directory: **Settings → Appearance → Themes → Manage**, search for **Dark Glass**, then **Install and use**.

By hand: download `manifest.json` and `theme.css` from the [latest release](https://github.com/oleksiimazurenko/obsidian-dark-glass/releases/latest) into `<your vault>/.obsidian/themes/Dark Glass/`, then pick **Dark Glass** in **Settings → Appearance → Themes**.

## Tune it

Every value worth changing is in the first block of `theme.css`. To override one without editing the theme, put it in a [CSS snippet](https://help.obsidian.md/snippets):

```css
body {
  --accent-h: 32;            /* accent hue (HSL); 210 for blue, 270 for violet */
  --accent-s: 85%;
  --accent-l: 64%;
  --glass-see-through: 0.62; /* 0 = solid cards, 1 = clear */
  --glass-graphite-top: 30 31 34;    /* backdrop gradient, rgb */
  --glass-graphite-bottom: 17 18 20;
  --glass-blur: 24px;        /* blur under floating layers */
  --glass-gap: 8px;          /* gap between cards */
  --glass-radius: 14px;      /* card corners */
}
```

## Licence

The theme is released under the [MIT License](LICENSE).

It embeds the [Montserrat](https://github.com/JulietaUla/Montserrat) typeface (Regular, Medium, SemiBold, Bold), © The Montserrat Project Authors, licensed under the [SIL Open Font License 1.1](OFL.txt).
