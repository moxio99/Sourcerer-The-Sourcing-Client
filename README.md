<p align="center">
  <img src="logo.png" width="130" alt="sourcerer" />
</p>

<h1 align="center">sourcerer</h1>
<p align="center"><i>type it, tab it, source it.</i></p>

<p align="center">
  <img alt="platform" src="https://img.shields.io/badge/platform-windows-0e1626?style=flat-square">
  <img alt="build" src="https://img.shields.io/badge/built%20with-python%20%2F%20tkinter-22d3ee?style=flat-square">
  <img alt="install" src="https://img.shields.io/badge/install-zero%20dependencies-fb923c?style=flat-square">
</p>

<br>

> heads up, this is a solo project and still rough in places. i built it because i was tired of opening the same six marketplace tabs by hand every time i needed a supplier. updates happen whenever i get to them.

<br>

## what it does

- **free-text search** — type anything, any case, any typo. nothing is matched against a local list, so nothing is ever "not supported."
- **ai enhance (optional)** — flip it on and your search gets cleaned up before it goes out: typos fixed, casing normalized, your custom requirements folded in. runs on groq, using your own api key, stored only on your machine. leave it off and everything still works exactly the same, just without the polish.
- **custom requirements** — add stuff like "min order 100" or "must be waterproof" and it gets woven into the search.
- **exact tab count** — the slider is a promise now. ask for 8 tabs, get 8 tabs, even if your region filter narrows the pool.
- **region filter** — toggle regions on, then pick whitelist (only these) or blacklist (everything but these).
- **your real browser** — every result opens as a normal tab. sourcerer holds nothing and tracks nothing.
- **one exe** — no installer, no python, no background service.

<br>

## using it

1. run `sourcerer.exe`.
2. type what you're sourcing.
3. *(optional)* add any custom requirements.
4. drag the slider for how many tabs you want.
5. *(optional)* toggle regions, pick whitelist or blacklist.
6. *(optional)* turn on ai enhance in settings with your own groq key.
7. hit **search suppliers**.

that's it. no accounts, no onboarding.

<br>

## the sourcing network

| source | region |
|---|---|
| alibaba | global |
| aliexpress | global |
| etsy | global |
| indiamart | india |
| tradeindia | india |
| thomasnet | usa |
| ebay | usa |
| amazon | usa |
| made-in-china | china |
| dhgate | china |
| amazon uk | europe |
| amazon germany | europe |
| ebay uk | europe |
| amazon uae | middle east |
| rakuten japan | asia-pacific |
| ebay australia | asia-pacific |

<br>

## installing

no installer, no dependencies. just the exe.

1. grab `sourcerer.exe` from this repo.
2. run it.
3. windows smartscreen might flag it since it isn't code-signed. click **more info → run anyway**.

<br>

## about the ai bit

ai enhance is off by default and needs your own free groq api key (get one at console.groq.com) — sourcerer never ships with a key baked in, and nothing gets sent anywhere unless you turn it on yourself. without it, sourcerer works exactly like before: your typed query, straight to every tab.

<br>

## how it behaves

doesn't phone home, doesn't collect analytics, doesn't store your searches. the only outside call it ever makes is to groq, and only if you've turned ai enhance on. every tab is just a normal search page on the destination site's own domain.

<br>

## found a bug?

message me on discord: **@.moxio**. sourcerer also pings you with this on launch, just in case.


