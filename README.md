<p align="center">
  <img src="logo.png" width="150" alt="Sourcerer" />
</p>

<h1 align="center">Sourcerer</h1>
<p align="center"><i>Autonomous supplier discovery, one search away.</i></p>

<p align="center">
  <img alt="platform" src="https://img.shields.io/badge/platform-Windows-0e1626?style=flat-square">
  <img alt="build" src="https://img.shields.io/badge/built%20with-Python%20%2F%20Tkinter-22d3ee?style=flat-square">
  <img alt="install" src="https://img.shields.io/badge/install-zero%20dependencies-fb923c?style=flat-square">
  
</p>

<br>

> Please note that this tool is solely developed by a single person, so it's not throughly tested, nor it is regularly updated. I built this tool to make it easier for those finding suppliers on products they're looking for, just by a click of a button. I don't regularly update this and it's pretty much in beta. If the searches are successful, that's a good thing, if it breaks, that's on me, I'm still working on this project. Please note this isn't abandoned, but it isn't my main focus aswell. 

<br>

Opening tons of tabs can be a pain. Getting redirected to outdated suppliers or not getting the exact product you browsed for is a headache. No one deserves that, and that's why, Welcome to Sourcerer

<br>

## Why it exists

Most sourcing tools make you pick from a dropdown of categories someone else already decided you need. This doesn't do that. There's no product catalog baked in, no list of "supported items" &mdash; the search box takes anything, in any case, and it just goes and opens the tabs. That was the whole point of building it: the second a tool makes you pre-teach it what you're allowed to search for, it stops being useful for the thing you actually needed it for. I'd rather ship something a little rough that searches for anything than something polished that only searches for what I thought to hardcode.

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

No installer, no dependencies, no Python required on your machine. Just the exe.

1. Grab `Sourcerer.exe` from this repository.
2. Run it.
3. Windows SmartScreen will probably flag it as unrecognized &mdash; that's just because it isn't code-signed (signing certificates aren't cheap for a solo side project). Click **More info → Run anyway**. It's not doing anything shady, I promise, but obviously don't take a stranger's word for it &mdash; the source is small enough to read yourself if you want to be sure.

<br>

## A note on how it behaves

It doesn't phone home, doesn't collect analytics, doesn't store your searches anywhere, and doesn't touch anything on your machine beyond opening your browser. Every tab it opens is just a normal search results page on the destination site's own domain. I have no interest in logging what you search for &mdash; I built this to save myself time, not to collect data.

<br>

## Known rough edges

Since this is beta and maintained by one person:

- Some marketplaces occasionally change how their search URLs work, which can make a tab land somewhere unexpected until I notice and fix it.
- Opening a lot of tabs at once depends on your browser and machine &mdash; it can lag on slower setups.
- No auto-update yet. New versions get posted here whenever they're ready, not on any set cadence.

If you hit something broken, it's genuinely useful to know about &mdash; open an issue and I'll get to it when I can.
