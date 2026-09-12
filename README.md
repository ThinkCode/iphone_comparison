# Should I Upgrade? — iPhone 18 Pro Max

A single-page, zero-dependency web toy: pick the iPhone in your pocket, get a
straight answer on whether the iPhone 18 Pro Max is worth it.

## Layout

The result is designed to land on a **single screen** — no scrolling on desktop
or iPad in either orientation. A top bar holds the picker, a wide verdict panel
sits above a four-tile metric grid, and the store links anchor the bottom. Below
900px wide (or on short viewports) it relaxes into a normal scrolling column.

## Artwork

The phones are **original CSS/SVG renderings**, not Apple product photography —
each generation in its signature colourway (Pacific Blue, Sierra Blue, Deep
Purple, Natural and Desert Titanium, Cosmic Orange, Burgundy). Apple's product
images are copyrighted and their use is not permitted here; the licensed route
for real product shots is Amazon's Product Advertising API, which requires
approved Associates credentials.

## What it does

- **Verdict score (0–100)** in an animated SVG ring, colour-coded green → amber → red.
- **Battery bar** comparing your model's video-playback hours against 45h.
- **Zoom visual** showing optical reach growing from yours to 8×.
- **Animated aperture diagram** for the new variable ƒ/1.48–4.0 main camera.
- **Four headline deltas** per model, plus native share / copy-link.

Deep links work: `index.html#15` opens straight to the iPhone 15 Pro Max verdict.

## Order links

Each verdict links out to Apple and to Amazon. The Amazon Associates tracking
ID lives in the `AMAZON_TAG` constant at the top of the `<script>` block in
`index.html`, currently `amznbargain-20`. The
affiliate disclosure required by the Associates Operating Agreement is rendered
under the buttons.

## Deploying

Served by GitHub Pages at **iphonecomparison.pricesearchr.com**. `CNAME` in the
repo root holds the custom domain; the DNS `CNAME` record for
`iphonecomparison` points at `thinkcode.github.io`.

GitHub Pages must be enabled in **Settings → Pages**, serving from the default
branch, and this content must be merged to that branch. Pages on a private
repository requires a paid GitHub plan; on the free plan the repo has to be
public for the site to serve.

## Running it

Open `index.html`. That's it — no build, no dependencies, no network calls.

## Data

iPhone 18 Pro Max figures come from the September 2026 spec comparison. Earlier
generations use Apple's published Pro Max specs. Not affiliated with Apple.
