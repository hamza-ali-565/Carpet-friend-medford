# Carpet Friend Medford — Website Pages

Source HTML for the **Carpet Friend Medford** website (carpetcleaningmedfordoregon.com), a carpet cleaning company serving Medford, Oregon and Jackson County.

Each page is built as a self-contained WordPress "Custom HTML" block (`<!-- wp:html -->`) so it can be pasted directly into the WordPress block editor. Styling is inline or scoped via a `<style>` block per file — there is no shared build/bundle step.

## Structure

Each top-level folder is one page or blog post and contains a single `.html` file matching WordPress's HTML-block format:

- **Core pages**: `Homepage`, `About`, `Contact`, `FAQ`, `Feedback`, `Best-Cleaners`
- **Layout partials**: `Header`, `Footer`, `Stick-Footer` — reused across pages, pasted into each page's header/footer block in WP
- **Service pages**: `Air-Duct-Cleaning`, `Carpet-Repair`, `Carpet-Stretching`, `Dryer-Vent-Cleaning`, `Hardwood-Floor-Cleaning`, `Natural-Stone-Cleaning`, `Stair-Carpet-Cleaning`, `Water-Damage-Restoration`
- **Location/service-area pages**: `Central-Point`, `Eagle-Point`, `Gold-Hill`, `Jacksonville`, `Phoenix`, `Rogue-River`, `Talent`, `White-City`
- **Legal pages**: `Privacy-Policy`, `Terms-Conditions`, `Disclaimer`
- **Blog posts**: all folders prefixed `Blog-*` (e.g. `Blog-Pet-Urine`, `Blog-Wildfire-Smoke-Smell`, `Blog-Cost-Guide`)
- **`_implementation`**: planning/implementation notes and PDFs used while building out the site (not deployed)

## Conventions

- Colors, fonts, and component styles (hero, footer, cards, buttons) are defined per-file using CSS custom properties (e.g. `--navy`, `--accent`, `--sky`) so each page can be pasted independently into WordPress without missing styles.
- Business info used across pages: phone `(458) 302-0101`, address `1600 Delta Waters Rd, Medford, OR 97504`, hours Mon–Fri 8am–6pm, Sat 9am–4pm.
- To update sitewide elements (nav, footer links, social links), edit `Header/header.html` and `Footer/footer.html`, then re-paste into each page that embeds them.

## Usage

1. Open the relevant folder's `.html` file.
2. Copy its contents.
3. In WordPress, add a **Custom HTML** block on the target page and paste.
