# Gerald Chang

Developer. I build macOS tools that respect the machine they run on.

**Now** — Software engineer at Enroute Tech in Melbourne, on a fleet
logistics platform: PHP microservices and two Flutter apps shipping on iOS and Android. On my own
time I build macOS and developer tooling.

*Updated September 2026.*

[Site](https://personal-site.dezhengchang.workers.dev) · [LinkedIn](https://www.linkedin.com/in/de-zheng-chang) · <dezhengchang@gmail.com>

---

### [CreativeNotch](https://github.com/GcdZ03/CreativeNotch) — Swift, SwiftUI, macOS 26+

Turns the MacBook notch into something useful, without the battery drain.

A notch app is ambient software: it sits under the menu bar for as long as the machine is on, and almost none of that time is spent looking at it — so its idle cost is the only cost that matters. One rule, written down before the first module: no subsystem runs when it isn't needed, enforced centrally rather than trusted to each module. `ARCHITECTURE.md` names four constructs as not allowed — an unconditional `Timer`, a permanently installed global event monitor, cursor-position polling, and an audio tap. The assumption is that if you think you need one, there's a notification you haven't found yet.

Shipped v0.5.0.

### [personal-site](https://github.com/GcdZ03/personal-site) — Astro, Tailwind, Cloudflare

The site linked above. Zero JavaScript shipped, served as an assets-only Cloudflare Worker, so nothing runs per request. Adding a project is one Markdown file, and the build fails with a readable error if the frontmatter is wrong.

---

**Building next:** `ctxlint` — a linter for AI agent context files (`CLAUDE.md`, `AGENTS.md`, Cursor rules) that catches drift against the repo they describe: dead paths, missing scripts, stale sections, instructions contradicted by the project's own config. Public once it works on something other than my own repos.
