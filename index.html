# Counselling Tool

A single directory for PW's counsellor-facing consoles — MIP, NEET Dropper, JoSAA (IIT/NIT/IIIT), and Defence Wallah — opened from one hub, each running exactly as its own team built it.

> Internal counsellor enablement tool. Not for student or public distribution.

## Structure

```
counselling-tool/
├── index.html          # the hub — directory, search, greeting, opens each tool in-page
└── tools/
    ├── mip.html         # MIP with RTS Console (AY 26-27)
    ├── neet.html        # NEET Dropper Counsellor Journey
    ├── josaa.html        # JoSAA 2026 Counsellor Console
    └── dw.html          # Defence Wallah Counsellor Journey
```

Each tool is a fully independent, self-contained HTML file. `index.html` never modifies them — it just lists them and loads the one you pick into an iframe.

## Running it

**Locally:** open `index.html` directly in a browser, or serve the folder for the most reliable experience:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000/index.html
```

**GitHub Pages:** push this folder to a repo, enable Pages on the branch/root, and `index.html` will work as-is — the tool cards load `tools/<name>.html` by relative path, exactly like any static site.

## Adding a new tool

1. Drop the new tool's HTML file into `tools/`.
2. Open `index.html`, find the `TOOLS` array near the top of the `<script>` block, and add one entry:

```js
{
  id: "yourtool",
  org: "TEAM NAME",
  name: "Tool Display Name",
  tagline: "Short one-liner",
  desc: "A sentence describing what it actually does.",
  tags: ["Real feature", "Real feature"],
  footLeft: "e.g. 5-step flow · 2026",
  accent: "#123456", soft: "#EEF1FA",
  file: "tools/yourtool.html"
}
```

That's it — the hub renders its card and wiring automatically.

## Updating an existing tool

Replace the file in `tools/` with the new version (same filename). Nothing else needs to change unless the tool's name, tagline, or feature tags are different — in which case update that one object in the `TOOLS` array.

## Voice / read-aloud feature

Each tool has a small 🔊 button injected next to its section headings, plus a floating control panel (bottom corner) with an EN/HI toggle and Stop. It uses the browser's built-in Web Speech API — no external service, no audio files.

- It reads the real, on-screen text of that section (and picks up sections that only appear after a click, e.g. selecting a cohort or batch tab).
- Tap a playing button again to stop; tap it again to replay.
- **HI mode switches the voice, not the language of the text.** It uses a Hindi text-to-speech voice where the visitor's device has one, but it still reads the actual English content on the page — it does not translate.
- In NEET, a collapsed section's mic will only read its heading until the section is expanded (that content is hidden from the page itself until then).

The module lives inline at the bottom of each `tools/*.html` file, wrapped in an IIFE as `window.PWVoice`, and does not touch or rely on any of that tool's own code.

## Notes

- No build step, no dependencies beyond two Google Fonts loaded over CDN. Everything else is plain HTML/CSS/JS.
- Quick-link URLs in the hub's top bar point to real sheets referenced inside `mip.html` (the live test-planner sheet and the PW Test Schedule Console) — nothing fabricated.
