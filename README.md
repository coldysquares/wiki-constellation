# Wiki Constellation

Wiki Constellation is an interactive browser explorer for walking outward from an English Wikipedia article through the pages it links to.

Enter a person, place, work, or idea. The matching Wikipedia article becomes the origin point, and its outgoing links become the surrounding field. Select a node to inspect it, open the source article, or move one layer deeper.

## What it is

- Standalone browser application
- Vanilla HTML, CSS, and JavaScript
- Live data from the MediaWiki Action API
- Small Vercel serverless endpoint for bounded Wikipedia lookup
- No account or local database required

## Project structure

- `index.html` — application shell and interface
- `styles.css` — responsive layout and visual system
- `app.js` — graph interaction, search, navigation, and rendering
- `api/wiki.js` — bounded English Wikipedia lookup endpoint
- `vercel.json` — deployment routing/configuration

## Data model

A connection means only that the current origin article contains an outgoing link to another Wikipedia page. It does not imply causality, agreement, endorsement, kinship, or any stronger semantic relationship.

## Deployment

This repository is intended to be the standalone source for Wiki Constellation. The serverless Wikipedia endpoint requires a host that supports the included Vercel function.

The public deployment should be connected directly to this repository so the repository, deployment, and public URL share one canonical source.
