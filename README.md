<p align="center">
  <img src="assets/logo.png" width="150" alt="Sourcerer" />
</p>

<h1 align="center">Sourcerer</h1>
<p align="center"><i>Autonomous supplier discovery, one search away.</i></p>

<p align="center">
  <img alt="platform" src="https://img.shields.io/badge/platform-Windows-0e1626?style=flat-square">
  <img alt="build" src="https://img.shields.io/badge/built%20with-Python%20%2F%20Tkinter-22d3ee?style=flat-square">
  <img alt="install" src="https://img.shields.io/badge/install-zero%20dependencies-fb923c?style=flat-square">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-1690a6?style=flat-square">
</p>

<br>

A solo developed tool, built out of frustration with how manual, slow, and repetitive supplier sourcing has become. Sourcerer takes whatever you type &mdash; a product, a material, a spec, a part number, anything &mdash; and instantly fans it out across a curated network of global marketplaces and B2B directories, opening each one in its own browser tab, ready to compare. No sign-up. No predefined product database. No limits on what you're allowed to search. Type it, tab it, source it.

<br>

## Why it exists

Most sourcing tools make you pick from a dropdown of categories they've already decided you need. Sourcerer doesn't work that way. There is no product catalog baked into it, no list of "supported items" &mdash; the search box takes anything, in any case, and the tool figures out where to point you. That's the whole idea: **the moment you have to pre-teach a tool what it's allowed to search for, it stops being useful for the thing you actually needed it for.**

<br>

## What it does

- **Free-text search** &mdash; type anything, in any case. Nothing is matched against a local database, so nothing is ever "not supported."
- **Tab slider** &mdash; drag to decide how many supplier tabs open at once, from a quick 1-tab check to a full sweep of the network.
- **Region control** &mdash; flip regions on with a switch, then choose whether that selection is a *whitelist* (only these) or a *blacklist* (everything but these). Leave nothing selected and every region is in play.
- **Opens your real browser** &mdash; every result lands as a normal tab in your default browser. Sourcerer itself holds nothing, tracks nothing, and closes the moment you close it.
- **One executable** &mdash; no installer, no Python runtime, no background service. Download it, run it, done.

<br>

## Using it

1. Launch `Sourcerer.exe`.
2. Type what you're sourcing into the search bar.
3. Drag the slider to set how many tabs you want opened.
4. *(Optional)* Toggle regions on and choose Whitelist or Blacklist.
5. Hit **Search Suppliers**. Your browser opens with a tab per source, already searching.

That's the entire workflow. No accounts, no setup screens, no onboarding.

<br>

## The sourcing network

Sourcerer doesn't scrape or index anything &mdash; it builds a live search URL for each source below and hands it straight to your browser, so every result you see is fetched directly from that marketplace itself, in real time.

| Source | Region |
|---|---|
| Alibaba | Global |
| AliExpress | Global |
| Etsy | Global |
| IndiaMART | India |
| TradeIndia | India |
| ThomasNet | USA |
| eBay | USA |
| Amazon | USA |
| Made-in-China | China |
| DHgate | China |
| Amazon UK | Europe |
| Amazon Germany | Europe |
| eBay UK | Europe |
| Amazon UAE | Middle East |
| Rakuten Japan | Asia-Pacific |
| eBay Australia | Asia-Pacific |

<br>

## Region filtering, explained

The toggles above the search button don't hide sources from a list &mdash; they change which of the sources above are eligible before the tab count is applied.

- **Nothing toggled** &mdash; every region is eligible. This is the default.
- **Whitelist mode** &mdash; only the toggled regions are eligible. Flip on *India* and *USA* to source domestically, ignore the rest.
- **Blacklist mode** &mdash; every region *except* the toggled ones is eligible. Flip on *China* in Blacklist mode to search everywhere else.

The tab slider then pulls from whatever pool that leaves, always in the same diversified order, so a small tab count still spreads across regions instead of clustering on one.

<br>

## Installing

No installer, no dependencies, no Python required on your machine.

1. Grab `Sourcerer.exe` from this repository.
2. Run it.
3. Windows SmartScreen may flag it as unrecognized, since it isn't code-signed &mdash; this is expected for an independently built tool. Click **More info → Run anyway**.

<br>

## A note on how it behaves

Sourcerer never phones home. It doesn't collect analytics, doesn't store your searches, doesn't need an internet connection to start, and doesn't touch anything on your machine beyond opening your browser. Every tab it opens is a standard search results page on the destination site's own domain &mdash; you're always in control of what happens after that.

<br>

## License

MIT &mdash; use it, fork it, point it at whatever you're sourcing.

<p align="center"><sub>Built solo. No team, no roadmap meetings &mdash; just a tool that got made because it needed to exist.</sub></p>
