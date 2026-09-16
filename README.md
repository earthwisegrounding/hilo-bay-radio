# Hilo Bay Radio

A single-page site for KHIB 88.1 FM, a fictional radio station in Hilo, Hawaiʻi. Bub, the morning host, is an ElevenLabs conversational AI agent. Visitors tap **Call in to the show** and talk to him live.

## Run it locally

```bash
python3 -m http.server 8641
```

Then open http://localhost:8641. Serve it rather than opening the file directly so the browser will grant microphone access.

## Change the host

The agent is set on the `<elevenlabs-convai>` element near the bottom of `index.html`. Swap `agent-id` to point at a different ElevenLabs agent. The widget's labels live in the `text-contents` attribute, and its colors in the `elevenlabs-convai { --el-* }` CSS block.

The live clock uses the Pacific/Honolulu time zone and the weather line comes from Open-Meteo for Hilo Airport.
