# Acquisition Readiness Summary

A single-page calculator that converts a self-funded buyer's capital position into a reachable
deal size, the SDE that deal must produce, and the maximum multiple they can afford to pay.

Built as the Phase 1 prototype: no accounts, no stored data, no server. All computation runs
in the browser.

## Deploy to GitHub Pages

1. Create a repo (e.g. `acquisition-readiness`) and push `index.html` to the default branch.
2. Repo → **Settings** → **Pages**.
3. Source: **Deploy from a branch**. Branch: `main`, folder: `/ (root)`. Save.
4. Live in a minute or two at `https://<username>.github.io/acquisition-readiness/`.

No build step. No dependencies beyond a Google Fonts stylesheet.

## Before showing anyone

- Print to PDF and read it on a phone. The PDF is what a broker actually receives.
- Confirm the default rate against a current SBA 7(a) quote.
- Decide whether the 2.0–3.5× typical multiple band matches your target sector; it is set in
  `BAND_LO` / `BAND_HI` near the top of the script.

## What this is not

Not a prequalification, not a credit decision, not advice. Every input is self-reported and
unverified. SBA parameters used (10% minimum injection on a change of ownership, 1.25× DSCR
floor) reflect commonly published lender guidance and vary by lender and deal.

## Pages

- `index.html` — readiness worksheet and printable summary. The artifact for broker testing.
- `verify.html` — simulated lender verification flow. Demonstration only; persistently labeled,
  no data collected, no credit inquiry, fictional institutions.

Keep these distinct. The summary is what you hand a broker. The verification flow is what you
show an investor or a prospective partner to explain where the product goes.
