# Should I Upgrade? — iPhone 18 Pro Max vs iPhone Duo

A single-page, zero-dependency web toy: pick the iPhone in your pocket, get a
straight answer on whether the iPhone 18 Pro Max or the foldable iPhone Duo is
worth it.

Live at **https://iphonecomparison.pricesearchr.com**

## Two upgrade targets

A segmented control in the top bar switches the comparison between the
**iPhone 18 Pro Max** ($1,299) and the **iPhone Duo** ($1,999), Apple's first
foldable. Each pairing of current phone and target carries its own score,
verdict and supporting facts, and the metric tiles change with the target —
the aperture tile becomes an unfolded-screen tile for the Duo.

The Duo comparison reports regressions honestly: it reaches 2x optical where
recent Pro Max models reach 5x or 8x, and 31h video unfolded against the 18 Pro
Max's 45h. Those show in warning colour rather than being omitted.

## Your phone: Pro Max or standard

A second switch beside the picker chooses the line of the phone you own: the
**Pro Max** (12–17 Pro Max) or the standard **iPhone** (12–17). Switching keeps
the same generation. Each phone has its own verdict for both targets, 24 in
all. Standard models with no telephoto (12–14) gain reach on the Duo rather
than losing it, and the verdicts say so.

## Battery health

A toggle under the verdict, "My battery health is below 80%", adds advice by
generation: try a battery replacement first (16, 17), a new battery is a
stopgap (14, 15), or a new battery won't fix the rest (12, 13). It links to
Apple's battery service page and quotes no repair price.

## Deep links

The hash carries phone and target: `#15` opens the 18 Pro Max verdict for an
iPhone 15 Pro Max, `#15/duo` the Duo verdict, and a `b` prefix selects the
standard model (`#b14`, `#b14/duo`).

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
- **Ship date** for the Duo beside the store links.
- **Share preview**: `og.png` (1200×630, rendered from the site's hero) is set
  as `og:image` / `twitter:image`, so shared links show a card.

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
generations use Apple's published Pro Max specs.

Standard models use Apple's published figures — video playback: 12 17h,
13 19h, 14 20h, 15 20h, 16 22h, 17 30h; optical reach 1× on the 12–14 and 2×
optical-quality on the 15–17. The iPhone 17 was checked against
apple.com/iphone-17/specs.

iPhone Duo figures come from Apple's announcement (September 2026): 7.6in inner
and 5.4in outer Super Retina XDR at 3000 nits, A20 Pro, 48MP Fusion main and
ultra wide, 2x optical-quality zoom, 31h video unfolded / 44h on the cover
screen, 50% charge in ~20 minutes, Grade 5 titanium, IP68, eSIM only, 256GB-2TB,
Star White and Night Sky, from $1,999, released 23 October 2026.

Apple quotes no f-number for the Duo's main camera and lists aperture as not
applicable, so the page does not claim one.

Not affiliated with Apple.
