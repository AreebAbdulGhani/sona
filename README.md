# Sona

**The Neuroadaptive Accessibility Fabric for Adobe Express.**

Every accessibility tool on the market measures your design and hands you a score. Sona simulates how an ADHD, autistic, dyslexic, or low-vision mind will actually experience it — before a single human sees it — then generates an editable, brand-safe variant tuned to each.

Built on four layers:

| Layer | What it does |
| --- | --- |
| **Cognitive Digital Twin** | A live semantic graph of the document: reading order, hierarchy, saliency, information density, cross-page narrative context. |
| **Agent Swarm** | Attention (ADHD), Sensory (autism), Reading (dyslexia), and Vision (low vision / CVD) agents score the twin off-thread and stream a live Cognitive Load Score per neurotype. |
| **Neuroadaptive Variants** | One master design forks into per-neurotype versions as fully editable Express pages, with Firefly supplying brand-locked assets. |
| **Portfolio Mesh** | Kubernetes-style reconciliation across an entire team's projects — declare requirements once in `a11y-spec.json`, and every design heals when the rules change. |

## Contents

- `index.html` — single-page site (dark, dependency-free, self-contained)
- `Sona_Technical_Architecture_v1.pdf` — technical whitepaper
- `whitepaper/whitepaper.html` — whitepaper source (renders to the PDF via headless Chrome)

## Status

Pre-seed. A working proof of concept builds a semantic graph of a multi-page Express document and simulates attention flow for ADHD users. Public beta targeted for **September 2026**.

## Local preview

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

## Rebuilding the whitepaper PDF

```sh
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf="Sona_Technical_Architecture_v1.pdf" \
  "file://$PWD/whitepaper/whitepaper.html"
```

## Contact

Areeb Abdul Ghani — areebghani359@gmail.com — Bengaluru, India
