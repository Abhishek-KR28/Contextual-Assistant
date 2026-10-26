# Workbench AI

A local-first conversational assistant prototype with persistent browser-based conversations and document-aware responses.

## Run it

```powershell
cd C:\Windows\System32\my-ai-assistant
npm install
npm run dev
```

Then open the URL Vite prints (normally `http://localhost:5173`).

## Included

- A persistent, selectable conversation list backed by browser local storage.
- Conversation follow-ups retain the current conversation state.
- Text, Markdown, CSV, and JSON document uploads.
- Document summaries and retrieval for queries that ask for deadlines, action items, decisions, requirements, or names.
- Inline source labels for retrieved material.
- Explicit messaging when private information cannot be verified because no sources are available.
- Local history clearing and responsive layout.

## Important limitations

This starter does not yet call a hosted language model or a connected enterprise knowledge source. Its response layer is intentionally local and deterministic, so it cannot answer unrestricted general-knowledge questions or truly reason over a document corpus. Add a server-side AI provider integration and an authorized retrieval connector before using it for production or sensitive information. Keep API keys in server environment variables, never in the browser or source code.
