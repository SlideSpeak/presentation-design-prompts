# Contributing

Thanks for adding to the collection. A theme is a small folder of markdown — the work is getting the design system in the prompt right.

## Add a theme

1. Create a folder `prompts/<slug>/` where `<slug>` is lowercase and hyphenated (e.g. `prompts/midnight-pitch/`).
2. Add the two files (copy an existing theme like [`prompts/boardroom`](prompts/boardroom) as a starting point):
   - **`PROMPT.md`** — just the prompt, the text people paste into a chat. End it with `Use this theme for my slides. Ask me what the presentation is about first, then apply the theme to every slide.`
   - **`README.md`** — the theme page: a one-line description, a metadata line (category, style, fonts), preview thumbnails, the prompt in a `text` code block, the palette table, and the font list.
3. Add a `previews/` folder with a few rendered example slides as `.webp` (`0.webp`, `1.webp`, …). If you can't render them, open the PR without — the SlideSpeak team can add previews.
4. Add your theme to the [gallery in `README.md`](README.md) and the [index in `prompts/README.md`](prompts/README.md), under the right category.
5. Open a pull request.

## Quality bar

The prompts are the product. Hold the bar high:

- **Pin everything.** Exact hex values, named Google Fonts, set type sizes and spacing. Vague adjectives ("modern", "clean") don't survive a generation.
- **Include an avoid list.** End the prompt with what the model must *not* do (clip-art, gradients, extra colors, bullet walls). It keeps output consistent.
- **Bring a distinct layout grammar.** A recolor of an existing theme is not a new theme.
- **Use real fonts.** Every font must exist on [Google Fonts](https://fonts.google.com) so anyone using the prompt can load it.

## Homages and trademarks

Themes that reference a known house style (say, a consulting firm) must be framed as **unofficial homages** built from publicly documented conventions. They must not claim affiliation or reproduce protected logos and trademarks.
