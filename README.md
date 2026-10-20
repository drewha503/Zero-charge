# Zero Charge

Finds free public EV chargers near you, tuned for a Rivian. One HTML file, no build step, no backend.

**Live app:** enable GitHub Pages (Settings → Pages → Source: Deploy from a branch → `main` / root) and it serves at `https://drewha503.github.io/zero-charge/`.

## What it does

- Finds chargers from your phone's location, a typed city/ZIP, or a tap on the map.
- Pulls public stations from the U.S. Department of Energy [Alternative Fuels Data Center](https://afdc.energy.gov/) (US and Canada).
- Shows only stations whose operator pricing note says free, no cost, complimentary, or $0.
  Green = plainly free. Amber = free with a condition (paid parking, customers only, time limit).
  Stations with no pricing note are hidden unless you toggle "Show unknown pricing".
- Filters: DC fast / Level 2, and plug type. J1772 and CCS are on by default (native on R1T/R1S).
  Tesla/NACS and NEMA outlets are off by default (adapter or portable charger needed).
- One-tap Apple Maps or Google Maps directions.
- Every result set shows its fetch time. If a refresh fails, old results stay but are marked STALE.

## API key

Ships with the shared `DEMO_KEY`, good for a few dozen lookups per hour. For your own free key,
sign up at https://developer.nrel.gov/signup/ and paste it into Settings. It is stored only in your browser.

## Not a guarantee

Pricing comes from station operators and lags reality. Read the sign before you plug in.

## Add to Home Screen

Open the Pages URL in Safari on iPhone → Share → Add to Home Screen. It runs full screen like an app.
