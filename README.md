# error-screenshot-explainer

OCRs a screenshot of an error dialog and explains what it means and how to fix it, on-device. Built with [Tether's QVAC SDK](https://github.com/tetherto/qvac) — the model runs on-device, so nothing leaves your machine.

## What it does

OCRs a screenshot of an error dialog and explains what it means and how to fix it, on-device.

**QVAC functions used:** `loadModel`, `ocr` and `completion`.

![error-screenshot-explainer demo](demo.png)

## Why I built it

Relatives send me photos of error popups. Now I can send back an answer, not a question.

## Requirements

- Node.js >= 22
- `@qvac/sdk` `^0.19.0` (installed automatically via `npm install`)

## Install

```bash
git clone https://github.com/YURIIMII-byte/error-screenshot-explainer.git
cd error-screenshot-explainer
npm install
```

## Run

```bash
node index.js path/to/error-screenshot.png
```

See the comments at the top of `index.js` for the exact input this app expects. On first run, QVAC downloads the model it needs once and caches it locally; every run after that is fully offline.

## SDK version used

`@qvac/sdk` `0.19.1`

## License

MIT — see [LICENSE](LICENSE).
