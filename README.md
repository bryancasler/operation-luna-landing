# Operation Luna Landing

A single-file guide to dog-friendly studios near Meridian Hill Park, Washington, DC, with what a month really costs, a review score that discounts small samples, and the questions to ask before applying.

Everything lives in `index.html`. The share image is `operation-luna-landing-og.png`. There is no build step and nothing to install.

Published with GitHub Pages at https://bryancasler.github.io/operation-luna-landing/

Prices and deals move weekly; the figures are a mid-September 2026 snapshot. Nothing here is a quote.

## Rebuilding it for a new search

[prompt-interview.md](prompt-interview.md) has Claude rebuild this page for a two-cat search centered on a home in Virginia. Claude interviews you one question at a time, then researches the buildings and rebuilds the page.

1. Start a new chat on claude.ai with Claude Opus 5.5 Extra. Leave Research Mode off, and turn on web search and code execution.
2. Open [prompt-interview.md](prompt-interview.md), copy everything below the `---` line, and send it as your first message.
3. Answer the questions. Have a photo of the cats ready and decide on the GitHub Pages address before you start; Claude asks for both.
4. Once you confirm Claude's summary, it works through every neighborhood without checking in. If a reply stops partway, say "continue."
5. Claude hands back four files: `index.html`, the share image, a new `README.md`, and `.nojekyll`. Put them in a new GitHub repo and turn on GitHub Pages.
