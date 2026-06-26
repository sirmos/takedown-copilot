# Takedown Copilot

> AI tool that turns online impersonation into action, generates platform reports, DMCA notices, and step-by-step takedown letters in under 2 minutes. No lawyer needed.

Built at **Youth Code x AI Hackathon 2026** - Track 03: AI That Helps People.

**Live app:** https://takedown-copilot-ycxai.web.app

---

## The Problem

AI-generated impersonation is growing fast. Deepfake videos, voice clones, and fake accounts are being used to scam fans, destroy reputations, and spread misinformation, all using real people's faces and voices without their consent.

The biggest gap is not detection. The gap is what happens after someone finds a fake of themselves online. Most people have no idea what a DMCA notice is, where to report it on each platform, or what to say. So the fake content stays up.

Takedown Copilot fixes that.

---

## What It Does

You provide:
- Your name or creator handle
- The platform (YouTube, TikTok, Instagram, X, Facebook)
- The type of impersonation (deepfake video, voice clone, fake profile, AI image)
- A link to the content
- A short description of what happened

The app generates three things instantly:

1. **Platform report blurb** - ready to paste into the platform's in-app report form, with a platform specific tip
2. **Formal takedown email** - complete with subject line, legal language, your details, and the date
3. **Step-by-step checklist** - six concrete next steps in order

No sign-up. No account. Works on any device.

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (single file, no frameworks)
- **AI:** OpenRouter API (LLaMA 3)
- **Hosting:** Firebase Hosting
- **Search:** Google Custom Search API (coming soon)

---

## Running Locally

1. Clone the repo:
```bash
git clone https://github.com/sirmos/takedown-copilot.git
```

2. Open `public/index.html` in your browser

3. Add your own API keys in the config section at the top of the file:
```javascript
const OPENROUTER_API_KEY = "YOUR_OPENROUTER_API_KEY";
const SEARCH_API_KEY     = "YOUR_SEARCH_API_KEY";
const SEARCH_CX          = "YOUR_SEARCH_ENGINE_ID";
```

4. Get a free OpenRouter key at https://openrouter.ai

---

## Deploying to Firebase

```bash
npm install -g firebase-tools
firebase login
firebase deploy
```

---

## What's Next

- Re-enable the scan feature with a backend search
- School and parent report letters for cases involving minors
- Multi-language support
- One-click email sending from the app
- Case tracker for open takedown requests

---

## Built By

Sirmos | Youth Code x AI Hackathon 2026
