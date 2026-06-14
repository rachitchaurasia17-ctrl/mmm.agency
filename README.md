# MMM Agency

A different kind of marketing agency. More reach. More sales. More money.

Static one-page site. Tunnel intro, hero, approach, sticky-stacking services, redesigned content calendar, Groq AI chatbot.

## Local preview

Open `index.html` in a browser, or run:

```bash
npx serve .
```

A local server is recommended (the 4K background video and chatbot fetch behave better than under `file://`).

## Chatbot key (local only)

Create `config.js` next to `index.html` (gitignored):

```js
window.MMM_GROQ_KEY = 'gsk_your_key_here';
```

The key never gets committed. For production, move the Groq call behind a server proxy (Cloudflare Worker, Vercel function) and remove the client-side key entirely.

## Deploy

Drop the folder into Cloudflare Pages, Vercel, or GitHub Pages — no build step needed.
