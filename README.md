## Levelbrook Consulting

Principal-led Ruby on Rails & backend engineering practice — production features,
performance work, and practical AI/LLM tooling for product teams.
Available for contract / C2C engagements. Pacific Time, US.

**Site:** [consulting.levelbrook.com](https://consulting.levelbrook.com) · **Contact:** levelbrookteam@gmail.com · **Résumé:** [front-end (PDF)](https://github.com/tachyurgy/beacon-seo-dashboard/blob/master/resume/levelbrook-consulting-frontend-resume.pdf)

---

### Original projects

| Project | What it is | Live |
|---|---|---|
| [**beacon-seo-dashboard**](https://github.com/tachyurgy/beacon-seo-dashboard) | React SEO & Core Web Vitals dashboard — animated score gauges and charts hand-coded in SVG (no chart library), Core Web Vitals scored against Google's real thresholds, fully responsive, light/dark. | [beacon-seo.pages.dev](https://beacon-seo.pages.dev) · [writeup](https://consulting.levelbrook.com/writing/beacon-seo-dashboard-react/) |
| [**hey-claude**](https://github.com/tachyurgy/hey-claude) | On-device macOS voice wake word that dispatches a background coding agent (openWakeWord + MLX Whisper on Apple Silicon). | [writeup](https://consulting.levelbrook.com/writing/hey-claude-on-device-wake-word/) |
| [**levelbrook-hotwire-demo**](https://github.com/tachyurgy/levelbrook-hotwire-demo) | Rails 8 + Hotwire product workbench — realtime collaboration, inline editing, command palette, and live LLM streaming. | [demo.levelbrook.com](https://demo.levelbrook.com) |
| [**equipment-cluster**](https://github.com/tachyurgy/equipment-cluster) | Visual ML pipeline over 20k+ equipment photos: DINOv2 → UMAP → HDBSCAN → CLIP zero-shot labels → React viewer. | [viewer](https://tachyurgy.github.io/equipment-cluster/) |
| [**linguaguessr**](https://github.com/tachyurgy/linguaguessr) | "GeoGuessr for the ear" — hear native speech, name the language, place it on the map. Whisper-verified corpus served from the edge. | [lingua.levelbrook.com](https://lingua.levelbrook.com) |

### Ruby libraries — small, single-purpose, tested

- [**ai_stream**](https://github.com/tachyurgy/ai_stream) — Ruby encoder for the Vercel AI SDK Data Stream protocol; drive `useChat`/`useObject` from a Rails/Rack backend. ([writeup](https://consulting.levelbrook.com/writing/vercel-ai-sdk-data-stream-ruby/))
- [**picoglob**](https://github.com/tachyurgy/picoglob) — compile bash-style globs into reusable Ruby `Regexp`s; picomatch/minimatch for Ruby. ([writeup](https://consulting.levelbrook.com/writing/bash-globs-to-ruby-regexps/))
- [**fzy_score**](https://github.com/tachyurgy/fzy_score) — faithful Ruby port of the fzy/fzf scoring algorithm; returns a score *and* matched positions for highlighting. ([writeup](https://consulting.levelbrook.com/writing/fuzzy-match-scoring-in-ruby/))

### Engineering writing

Long-form, lived-in war stories on production Rails work — N+1 hunts, large-table
pagination, storage tiering, brittle integrations — at
[consulting.levelbrook.com/writing](https://consulting.levelbrook.com/writing/).

---

*Rails · Hotwire · Postgres · background jobs · production debugging · performance tuning · practical AI tooling.*
