# Prayer Mountain Ministry

Purple, gold and cream church website with a starter LiveKit audio connection.

## Netlify settings
- Base directory: blank
- Build command: blank
- Publish directory: `.`
- Functions directory: `netlify/functions`

Set these environment variables in Netlify (never commit secrets to GitHub):
- `LIVEKIT_URL` — LiveKit WebSocket URL beginning `wss://`
- `LIVEKIT_API_KEY` — LiveKit API key
- `LIVEKIT_API_SECRET` — LiveKit API secret; mark secret

After connecting the repository to Netlify, trigger a fresh deploy.

## Important before public launch
This is a starter implementation. The token endpoint currently allows any visitor who knows a room name to request a participant token. Add server-side room-code validation, rate limiting, and authenticated host/admin permissions before public use. Client-side microphone mute is not enforceable host moderation. Test with a small group first.
