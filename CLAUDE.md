# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file browser game — `tictactoe.html` — with no build step, dependencies, or server required. Open the file directly in any browser to run it.

## Architecture

Everything lives in `tictactoe.html`:

- **HTML** — 3×3 grid of `.cell` divs, a status line, scoreboard, and a reset button.
- **CSS** (inline `<style>`) — Dark theme (`#1a1a2e` background), X cells styled red (`#ff6b6b`), O cells teal (`#4ecdc4`), winning cells highlighted with a pulse animation.
- **JS** (inline `<script>`) — Plain vanilla JS. Game state is a 9-element array (`board`). Win detection iterates over 8 hardcoded winning lines (`WINS`). Scores persist in a `scores` object for the lifetime of the page session.
