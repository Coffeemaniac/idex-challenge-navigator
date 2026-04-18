# iDEX Challenge Navigator

A single-file, static navigator for India's **iDEX (Innovations for Defence Excellence)** open
problem statements — 209 challenges across four active tracks:

- **DISC 14** — 82 problem statements
- **ADITI 4.0** — 25 deep-tech problem statements
- **DRISHTI (DPSU-driven)** — 101 problem statements
- **iDEX Open Challenge** — 1 rolling problem statement

Source PDFs from the Defence Innovation Organisation (DIO) were extracted with
`pdftotext -layout`, parsed into structured JSON, and baked into the HTML. No build step,
no server, no dependencies — just open `index.html`.

## Features

- Filter by program, nodal agency, tech domain, bookmarks, or notes
- Full-text search across problem statement, brief, technology domains, application
- **Bookmarks** + **personal notes** persisted in localStorage
- **About Programs** overlay with tracks, grant ceilings, evaluation criteria, and deadlines
- **Shareable deep links** — every challenge has a unique URL via the hash fragment,
  e.g. `…/#DISC14-42`. Click _Copy Link_ in any challenge modal.

## Deep-link URL format

```
https://<host>/#<CHALLENGE_ID>
```

Examples:
- `#DISC14-1` — DISC 14, Problem Statement 1
- `#ADITI-10` — ADITI 4.0, Problem Statement 10
- `#DRISHTI-50` — DRISHTI, Problem Statement 50
- `#OPEN-1` — iDEX Open Challenge

Opening any of these URLs auto-opens the corresponding challenge modal on load.

## Local use

Just open `index.html` in a browser. That's it.

## License

Problem statement content is © Government of India / Ministry of Defence / DIO.
This navigator UI is provided as-is for convenience; no affiliation with iDEX / DIO.
