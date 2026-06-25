# Deep-Build Plan — LLM Apps & Agents

An interactive, single-file web document of a **12-week senior-track plan** for going
from *ships agents* to *rigorously good* at building LLM apps and agents.

It tracks your progress through five phases — measure what you have, make evals a
first-class discipline, build reliably under measurement, go below the API, and
synthesize the narrative — with checkable steps, per-phase and global completion,
and a live progress ring.

## View it

It's a standalone HTML file with no build step or dependencies (fonts load from
Google Fonts). Either:

```bash
open index.html            # macOS — opens in your default browser
```

or serve it locally:

```bash
python3 -m http.server      # then visit http://localhost:8000
```

## Features

- **Live progress ring** plus per-phase and global step/phase counts in the header.
- **Checkable steps and deliverables** for each phase.
- **"The shape" navigator** — click a phase to expand it and smooth-scroll to its card.
- **Expand/collapse** phase cards; **reset progress** in one click.
- **Persistence** — your progress is saved in `localStorage` (`dbp_state_v1`) and
  restored on reload.

## Structure

```
index.html                      The interactive document (the deliverable).
project/Deep-Build Plan.dc.html  Original design source (provenance only).
```

`index.html` is a dependency-free, vanilla-JS recreation of the design. The
`.dc.html` file under `project/` is the original prototype exported from
[Claude Design](https://claude.ai/design); it is kept for reference and is not
meant to run on its own.
