# RankMoviewiz 2026

A single-page, static HTML website that displays a personally curated, ranked list of the most anticipated/best films of 2026. Built by Koome The Dev.

## Overview

RankMoviewiz presents a "Top 10" style leaderboard of movies, each with a rank number, emoji poster placeholder, title, release/cast metadata, genre tags, and a personal rating score (out of 10, plus a star rating). The page has a dark, teal-and-forest gradient aesthetic with a subtle grain texture, serif display headings (Playfair Display), and a clean sans-serif body font (DM Sans).

## Features

- **Ranked movie list** — 10 movies ranked #1–#10, each with a score, star rating, and "New" / "Unreleased" status badge.
- **Genre filter bar** — Buttons for All, Horror, Drama, Thriller, Sci-Fi, Action, and Comedy (UI toggle only — see [Known Limitations](#known-limitations)).
- **Responsive layout** — Adapts spacing, font sizes, and grid columns for screens under 600px wide.
- **Visual polish** — Custom gradient background, SVG noise/grain overlay, hover states on movie cards, and highlighted styling for the top 3 (and especially #1) ranked entries.

## File Structure

```
movie-ranking.html   # Single self-contained file — HTML, CSS, and JS all inline
```

No external dependencies besides a Google Fonts import (Playfair Display & DM Sans).

## Usage

Just open `movie-ranking.html` directly in any modern web browser — no build step, server, or install required.

## Known Limitations

- The genre filter buttons currently only toggle their own `active` visual state (via inline `<script>`); they don't yet filter the movie list itself.
- Movie poster images are emoji placeholders rather than real artwork.
- Content (titles, ratings, cast) is hardcoded directly in the HTML rather than pulled from a data source.

## Possible Next Steps

- Wire up the filter buttons to actually show/hide movie cards by genre.
- Move movie data into a JSON array and render cards dynamically.
- Replace emoji placeholders with real poster images.
- Add a search box or sort-by-score control.

## Credits

Ratings and curation are based on the personal opinion of **Koome The Dev**.
