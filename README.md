# Text to Handwriting

Convert typed text into realistic handwritten pages (assignments, notes, letters) without uploading anything to a server.

Live: <https://crusher-labs.github.io/text-to-handwriting/>

## What it does

Five handwriting styles (Google handwriting fonts), blue/black/green ink, ruled or plain A4-proportioned paper, per-character jitter for a natural look, automatic multi-page flow for long text, and PNG downloads per page with no watermark.

## Privacy

This tool runs entirely in your browser. There is no server. No data is uploaded, no telemetry, no analytics. The only network requests fired are the page-load fetches for the framework's CSS / JS (from `cdn.jsdelivr.net` and `fonts.googleapis.com` / `fonts.gstatic.com`); your inputs and outputs never leave the tab.

## Framework / hosting

- Static HTML / CSS / JS deployed via GitHub Pages from this repo's `main` branch.
- UI chrome is the published `crusher-ui-kit` static contract; the pinned version and its SRI hashes are managed fleet-wide by `tools-hub/scripts/bump-kit.mjs`.

## Development

- Open `index.html` directly in a browser. No build, no dependencies.
- Or serve the parent workspace via the hub's preview server: `cd ../../tools-hub && npm run preview` then visit `http://127.0.0.1:8723/utility-tools/text-to-handwriting/`.

## License

MIT.
