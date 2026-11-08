# GCC Health Insurance Observatory

A regional, evidence-led observatory interface for detecting, documenting and monitoring signals across the six GCC health-insurance markets.

## Navigation model

The GCC landing page is the regional entry point. The geographic GCC map is an interactive country selector: select a country polygon, label or marker to open that country's observatory. The country directory cards provide a second accessible entry point.

All six country observatories use the same shared workflow. Selecting a country changes the market identity while preserving the common methodology. Country-specific evidence is added only after research and review.

## Unified observatory workflow

1. **External Signal Detection** — scan the wider environment without restricting discovery to predefined sectors.
2. **Signal Documentation & Evidence** — record original sources, publication and event dates, organizations, evidence, observation date and verification status.
3. **Cross-sector Connections** — test how signals may connect across insurers, TPAs, providers, employers, technology, regulation and other parts of the ecosystem.
4. **Impact & Opportunity Monitoring** — assess possible impact pathways, confidence and strategic or commercial opportunities, then monitor signals as evidence evolves.

**Continuous learning — Emerging Themes:** documented signals accumulate over time to reveal recurring patterns, emerging themes and changing market direction. New evidence can update any earlier stage.

## Current release

**Interactive GCC country entry + shared workflow**

- Preserves the GCC landing page and regional signal map.
- Renders country polygons and international boundaries from Natural Earth Admin 0 geography, redistributed as TopoJSON by `world-atlas` at 1:10m scale.
- Makes all six GCC country shapes, labels and markers interactive, with a clear instruction to select a country.
- Keeps a country directory as an alternative navigation route.
- Opens a shared country observatory view with the unified four-stage workflow and continuous-learning layer.
- Supports English and Arabic, including right-to-left layout and accessible map-control labels.
- Keeps the AI Observatory and timeline concepts out of the primary navigation until those views are ready for release.

## Evidence and limitations

The map uses Natural Earth country-boundary geography through the `world-atlas` TopoJSON distribution (Natural Earth 1:10m Admin 0, world-atlas 2.0.2 / Natural Earth 4.1.0). It is a regional reference map, not a cadastral or legal boundary authority. Natural Earth applies a de facto boundary policy; disputed alignments may differ from individual governments' claims. GCC country shapes, markers and labels are navigation controls, not evidence of signal volume or market activity. The map geometry is loaded from jsDelivr at runtime, so a network connection is required for the map to render.

No live monitoring, automated ingestion, database, API or evidence-verification workflow is implemented in this interface-only release. Country-specific signals, entities and sources must be added only after research and evidence review.

## Geographic data attribution

- Boundary source: [Natural Earth — 1:10m Cultural Vectors](https://www.naturalearthdata.com/downloads/10m-cultural-vectors/)
- Browser distribution: [world-atlas](https://github.com/topojson/world-atlas), a TopoJSON redistribution of Natural Earth 4.1.0.
- Boundary type: Admin 0 country polygons; 1:10m large-scale geography.
- Natural Earth data is public domain. The map is intended for regional market orientation, not legal or cadastral use.

## Research principles

- Discover signals openly; do not let predefined categories limit discovery.
- Preserve original sources and distinguish event date from observation date.
- Separate reported information from verified evidence.
- Test cross-sector connections rather than assume causality.
- AI may assist discovery and analysis; human review remains responsible for verification and final judgment.

## Run locally

Open `index.html` in a browser. No build step, backend or database is required. The geographic map loads D3 Geo, TopoJSON Client and the Natural Earth-derived `world-atlas` country data from jsDelivr.

## Roadmap

Future releases may add country-level evidence registries, structured source records, entity relationships, historical observations, GCC cross-market comparison and AI-assisted signal discovery. These capabilities are not yet implemented.
