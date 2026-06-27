# From Author to Orchestrator — Slidev deck

A 25-minute lecture on how AI and coding agents are redefining software engineering, for year 1–3 CS students. Minimal slides, one focal infographic each; all depth, citations, and discussion prompts live in the **presenter notes**.

## Run it

```bash
npm install
npm run dev        # opens at http://localhost:3030
```

Press **`p`** to toggle the presenter view (your speaker notes + the next slide). Arrow keys / space to advance.

## Export

```bash
npm run export        # → slides-export.pdf  (needs playwright-chromium, installs on first run)
npm run export-png    # → one PNG per slide
```

## Design system (`style.css`)

Color carries meaning, not decoration:

| token      | meaning                                            |
|------------|----------------------------------------------------|
| `--human`  | amber — the human: intent, judgment, productivity  |
| `--agent`  | cyan — the machine: agents, automation, AI gains   |
| `--warn`   | red — genuinely negative outcomes: slower, decline |

Type: **Space Grotesk** (display) · **IBM Plex Sans** (body) · **JetBrains Mono** (data + eyebrows).

To recolor the whole deck, edit the `:root` variables at the top of `style.css`.

## Editing

- Each slide is separated by `---`. Per-slide settings (e.g. `layout: center`) go in a small frontmatter block right after the separator.
- Speaker notes are the `<!-- ... -->` block at the end of each slide.
- The two SVG infographics (perception gap on slide 6, adoption-vs-trust on slide 7) are hand-drawn inline — tweak coordinates directly if you reflow them.
