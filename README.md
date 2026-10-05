# SpeakEase – Interview English Coach
Speech-enabled web app for CEFR-level (A1–C2) interview English practice with a non-judgmental growth score, grammar buddy and AI feedback.

**Stack:** HTML, CSS, JavaScript, Web Speech API, Netlify Functions (Node.js), Google Gemini API

## Deploy on Netlify
1. Get a free key from Google AI Studio.
2. Push this folder to a GitHub repo (never commit the key).
3. Netlify → Add new site → Import from Git → pick the repo (no build command, publish directory `.`).
4. Site configuration → Environment variables: add `GEMINI_API_KEY` (and optionally `GEMINI_MODEL`, default `gemini-2.5-flash-lite`).
5. Redeploy. If the AI is unavailable, the app falls back to rule-based feedback automatically.

## Security
The API key stays in the server function, never in the browser. Inputs are length-limited.
