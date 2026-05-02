# getfledge

Landing page for [Fledge](https://github.com/CorvidLabs/fledge) — one CLI for your entire dev lifecycle.

**Live:** [corvidlabs.github.io/getfledge](https://corvidlabs.github.io/getfledge/)

## What is Fledge?

Fledge is a single Rust binary that replaces your Makefile, shell scripts, and scattered tooling. Scaffold projects, run tasks, review code with AI, manage releases — all from one CLI with one config file.

- **Humans** get interactive prompts, colored output, and pretty diffs
- **AI agents** get structured JSON — no parsing hacks needed
- **New hires** get guided setup and zero tribal knowledge

## Stack

- Static HTML + CSS (no framework, no build step)
- GitHub Pages deployment
- Inter + JetBrains Mono fonts
- IntersectionObserver scroll animations

## Local development

This repo eats its own dog food — tasks are defined in `fledge.toml`.

```bash
# Serve locally
fledge run serve            # python3 http.server on :8000
fledge run serve-bun        # bunx serve alternative

# Validate before pushing
fledge run validate         # html-validate on index.html
fledge lanes run ci         # format-check + validate + links
```

Open `http://localhost:8000` in your browser.

> Don't have fledge yet? `cargo install fledge` or `brew install CorvidLabs/tap/fledge`.

## Deploy

Pushes to `main` auto-deploy via GitHub Pages.

## Links

- [Fledge repo](https://github.com/CorvidLabs/fledge)
- [Documentation](https://corvidlabs.github.io/fledge/)
- [Plugins](https://github.com/orgs/CorvidLabs/repositories?q=fledge-plugin)
