# Investments Page Enhancement Design

## Overview

Enhance the investments page with concise descriptions and subtle fade-in animations.

## Changes

### 1. Updated Descriptions (6-10 words each)

| Company | Description |
|---------|-------------|
| AMASS | Clean botanical spirits and body care products. |
| DFNS | Secure crypto custody infrastructure as an API. |
| Kubik | Turns plastic waste into low-carbon buildings. |
| Asaak | Asset financing for tools and transport across Africa. |
| Bold | The bitcoin-backed credit card. |
| Prometheus | Renewable fuels from solar and air. |
| Go | Subscribe to cars in minutes. |
| Republic | Now everyone can invest in startups. |

### 2. Pure Fade Animation on Scroll

**Behavior:**
- Cards start invisible (opacity: 0)
- As each card enters the viewport, it fades to visible (opacity: 1)
- Transition duration: 0.6s with ease timing
- Cards appear individually as user scrolls

**Implementation:**
- Add `.fade-in` class to each investment card
- Inline script uses Intersection Observer to add `.visible` class on viewport entry
- CSS handles the transition
- Fallback: cards display normally if JavaScript is disabled

## Files Modified

- `src/pages/investments.astro` - update descriptions, add fade-in class, add script and styles
