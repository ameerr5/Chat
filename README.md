# Vercel + GitHub Gist Chat (Minimal)


This repository is a minimal chat demo built with Next.js that persists messages inside a GitHub Gist. It's designed for easy deployment to Vercel and storage via GitHub (so you can use "GitHub" as the backend as requested).


## How it works
- The front-end (Next.js) polls `/api/messages` every 2 seconds to fetch messages.
- Sending a message calls `/api/messages` POST — the API reads the `messages.json` file inside a GitHub Gist, appends the message, and updates the gist.