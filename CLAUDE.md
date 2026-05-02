# CLAUDE.md

## My coding knowledge level

I'm a novice coder. When you explain things, use plain language and gloss any jargon the first time it shows up (e.g. "CNAME = a DNS record that says 'this name points at that name'"). Default to the simplest viable approach — this site is a single `index.html`, not a framework, and I'd like to keep it that way unless I ask otherwise. I go by "memi" on this site.

## My preferred response style

- Keep replies short. One sentence saying what you're about to do, then do it.
- Don't narrate your thought process; just show the result.
- For setup steps (DNS, GitHub, registrar UIs), give numbered click-by-click instructions and screenshot-friendly directions.
- When I give a terse instruction ("no underline", "put it on the website"), act on it directly — don't re-pitch design choices.
- If something I said is ambiguous, ask one focused question instead of guessing.

## What we built (2026-05-01)

- Created `index.html`: dark brown background (`#2b2522`), light-grey (`#c9c9c9`) Helvetica Bold email link anchored to the lower-right corner. Letters are spaced out (`letter-spacing: 0.12em`), no underline.
- Font size is responsive: `clamp(18pt, 6.5vw, 48pt)` so it caps at 48pt on desktop and shrinks to a readable size on iPhone.
- Set up custom domain `m3m1.com` via a `CNAME` file in the repo + GoDaddy DNS (four `A` records on `@` → GitHub's IPs `185.199.108–111.153`, and one `CNAME` on `www` → `gituserm10.github.io`).
- Site is live at https://m3m1.com (HTTPS auto-provisioned by GitHub). `gituserm10.github.io` and `www.m3m1.com` both redirect there.
