# Gerald Chang

Developer. I build macOS tools that respect the machine they run on.

[Site](https://personal-site.dezhengchang.workers.dev) · [LinkedIn](https://www.linkedin.com/in/de-zheng-chang) · <dezhengchang@gmail.com>

---

### [CreativeNotch](https://github.com/GcdZ03/CreativeNotch) — Swift, SwiftUI, macOS 26+

Turns the MacBook notch into something useful, without the battery drain.

A notch app is ambient software: it sits under the menu bar for as long as the machine is on, and almost none of that time is spent looking at it — so its idle cost is the only cost that matters. One rule, written down before the first module: no subsystem runs when it isn't needed, enforced centrally rather than trusted to each module. `ARCHITECTURE.md` names four constructs as not allowed — an unconditional `Timer`, a permanently installed global event monitor, cursor-position polling, and an audio tap. The assumption is that if you think you need one, there's a notification you haven't found yet.

Shipped v0.5.0.

### [personal-site](https://github.com/GcdZ03/personal-site) — Astro, Tailwind, Cloudflare

The site linked above. Zero JavaScript shipped, served as an assets-only Cloudflare Worker, so nothing runs per request. Adding a project is one Markdown file, and the build fails with a readable error if the frontmatter is wrong.

---

**In progress:** a linter for AI agent context files that catches drift against the repo, a terminal-native API client with plain-text request files, and a tool that attaches an agent's reasoning to the pull request it opened. Public when they're worth reading.
