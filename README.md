# VIDAI AI — Responsive Trust & Safety Website

A mobile-first, single-page website prototype for Android, iOS, tablets, and desktop browsers.

## Run it
1. Unzip this folder.
2. Open `index.html` in a modern browser, or upload the files to a static host.
3. No package installation or build step is required.

## Working in this prototype
- Responsive navigation and feature sections
- URL structure inspection (local heuristic only)
- Claim verification checklist generator
- Scam-language warning phrase checker
- Local check history using browser localStorage
- Export history to JSON
- Clear history and toggle history saving
- Mobile-responsive layout

## Important honesty / production limitations
This is a functioning **front-end prototype**, not a fully deployed production service. It does NOT yet connect to:
- Live URL reputation or malware databases
- A live web search / fact-checking API
- An AI model API
- User accounts, cloud sync, or a server database
- Browser extension or push notification service
- Real analytics

The demo deliberately does not claim to know whether a site or claim is 100% safe/true. The URL and message checks are simple heuristics, and results can be wrong. The claim tool generates a verification checklist rather than verifying the claim itself.

## To make it a real production service
Build a backend API (for example, FastAPI or Node.js), connect vetted URL reputation services and a search/source retrieval system, add rate limits and abuse protection, keep API keys on the server, create privacy/retention policies, and test with real users. Add authentication only if cloud accounts are needed. Never put private API keys in frontend JavaScript.

## Deployment
You can deploy this static prototype on a static hosting provider by uploading `index.html`. For a custom domain, configure DNS and HTTPS with the host. Hosting and domain purchase are not included in this zip.
