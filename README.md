# 🎧 Spotify Top 50 Analytics Dashboard

An interactive Power BI dashboard exploring the Global Top 50 Spotify tracks — built to go past static charts into a dynamic, user-driven analytics experience.

## Overview
Single-page (1280×720) dashboard analyzing track-level popularity, album composition, explicit content, and release-year trends across the Top 50 dataset.

## Key Features
- **Dynamic Field Parameters** — core chart(s) let the user switch the underlying measure/dimension on the fly, avoiding duplicate pages for each cut of data
- **Custom DAX measures**: `Distinct Songs`, `Avg Popularity`, `Avg Duration Minutes`, `Explicit Songs`, `Non-Explicit Songs`, `Avg Popularity by Album Type`
- **KPI cards** for at-a-glance totals (song count, avg duration, avg popularity)
- **Donut breakdowns**: songs by album type, explicit vs. non-explicit split, songs by year, avg popularity by album type
- **Clustered bar/column charts**: songs by artist, popularity by song
- **Searchable track slicer** with live album artwork thumbnails
- **Custom icon-driven UI** (play / pause / back imagery) for a music-player-inspired look instead of default Power BI styling

## Data Model
- Core fact table: `Top-50-World` (song, artist, album_type, popularity, duration, explicit flag, album_cover_url)
- Auto date table for year-based analysis
- Separate measures table for centralized DAX logic

## Tech Stack
- Power BI Desktop
- DAX (measures, field parameters)
- Power Query (data shaping)

## Preview
*(add a screenshot or GIF of the dashboard here)*

## How to Use
1. Download `spotify_dashboard.pbix`
2. Open in Power BI Desktop
3. Use the field-parameter slicer to switch chart metrics; use the search slicer to filter by track
