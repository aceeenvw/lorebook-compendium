# The Lorebook Compendium

A short, visual reference for what belongs *inside* a lorebook — and what is better kept on the character card. Written for beginners building bots in **SillyTavern** and **JanitorAI**.

> A small archive of what one person picked up over months of trial, error, and stubbornness while making bots. Not gospel — just notes from a workbench.

## What it is

A single self-contained HTML page (`lorebook-compendium.html`) covering:

1. What is a lorebook?
2. What belongs where (card vs lorebook split)
3. The three layers — World / Character / User
4. Common entry categories
5. Anatomy of an entry
6. Keywords — ST regex vs JAI wildcards
7. Quick rules — do / don't
8. Build order
9. Card field cheat-sheet
10. Where do tokens go? (budget visualization)
11. Common mistakes & fixes
12. Glossary
13. Further reading

## Stack

- **One file**, no build step, no dependencies
- ~73 KB total
- Self-hosted fonts via Google Fonts (EB Garamond + JetBrains Mono)
- ~158 bytes of inline JS for the hamburger menu (CSP-hashed)
- Mobile-first responsive
- WCAG-conscious (focus rings, reduced-motion, ARIA labels, semantic HTML)

## Security

Locked down with a strict Content Security Policy:

- `default-src 'none'`
- `script-src` whitelisted by **SHA-256 hash only** (no `unsafe-inline`, no remote scripts)
- `base-uri 'none'`, `form-action 'none'`, `frame-ancestors 'none'`
- All external links use `rel="noopener noreferrer external"` + `target="_blank"`
- `<meta name="referrer" content="no-referrer">`
- Zero analytics, trackers, or pixels

If you self-host, mirror the CSP as an HTTP header at the host level for defense-in-depth.

## Usage

Open `lorebook-compendium.html` directly in any modern browser, or drop it on a static host:

- **Vercel** — `vercel deploy`
- **GitHub Pages** — push to `main`, enable Pages
- **Cloudflare Pages** — connect repo, no build command needed
- **Neocities** — drag and drop

## Disclaimer

This is one person's system. Other creators do it differently — that's fine. The way I build things now will probably look different in six months, and this file might quietly change with it. Take what helps, leave what doesn't.

Read the official docs for ground truth:

- [SillyTavern Documentation](https://docs.sillytavern.app/)
- [JanitorAI Help Center](https://help.janitorai.com/en/category/user-guides-vtspde/)

## License

Do whatever you want with it.

---

Made by [aceenvw](https://janitorai.com/profiles/895c6c07-6a53-4420-bff5-b874db870b32_profile-of-aceenvw) ☘
