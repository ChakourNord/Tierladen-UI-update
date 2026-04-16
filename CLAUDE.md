# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static single-page website for **Tiernahrung LOB** — a premium German pet food specialty shop in Aachen. No build system, no npm, no frameworks.

## Running the Project

Open `index.html` directly in a browser. No server, build step, or install required.

## Architecture

**Single file**: All HTML, CSS, and JavaScript live in `index.html` (~1,600 lines).

- **Lines 11–42**: CSS custom properties (design tokens) — colors, typography, spacing, shadows, border-radius
- **Lines 43–1536**: HTML structure (nav, hero, category pills, product grid, concept section, blog, deals, footer)
- **Lines 1537–1594**: Vanilla JS — hero word animation (`setInterval`), category pill active states, wishlist heart toggle, scroll-reveal via `IntersectionObserver`

## Design System

CSS variables follow a semantic token pattern. The primary brand color is `--color-primary: #ff385c` ("Rausch Red"). Font: `Plus Jakarta Sans` from Google Fonts. All visual changes should go through the CSS custom properties at the top of the `<style>` block rather than hardcoded values.

## Language

UI text is in German. Keep all user-facing text in German when editing or adding content.
