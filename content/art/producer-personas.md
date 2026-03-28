# Producer Personas

Technical specifications for consistent production quality across AI-generated artwork.

---

## Print Producer

**Output:** High-resolution static images for book chapters, gallery display, and physical prints.

**Resolution:** Minimum 2048x2048px. Chapter headers at 16:9 aspect ratio (2560x1440 or higher). Gallery pieces at 1:1 or 4:5.

**Color profile:** sRGB for digital, CMYK-safe palette for print. Avoid pure neon — shift toward analog warmth.

**File format:** PNG (lossless) for masters. JPG at 95% for web/repo storage.

**Consistency rules:**
- All chapter art shares a cohesive palette — muted earth tones as base, with accent color tied to the chapter's emotional register
- Grain/texture layer applied uniformly across the series
- No text baked into images — titles are handled in layout
- Each piece must read at both full size and thumbnail (GitHub preview)

---

## Motion Producer

**Output:** Animated or interactive pieces — HTML visualizations, looping sequences, visual companions to music.

**Format:** HTML/CSS/JS for interactive (see `gallery.html`, `living-geometry-radial.html`). GIF or MP4 for loops.

**Frame rate:** 30fps for loops. Interactive pieces should target 60fps.

**Consistency rules:**
- Same color palette as print work
- Motion should feel organic — no hard cuts, no mechanical easing
- Interactive pieces must degrade gracefully (static fallback)
- File size conscious — these live in a git repo

---

## Album Art Producer

**Output:** Artwork for seeds, covers, and collabs.

**Resolution:** 3000x3000px (streaming platform standard). Square format only.

**Style:** Uses The Transmitter persona as default. High contrast, graphic, legible at 300x300px thumbnail.

**Consistency rules:**
- Band name treatment consistent across all releases
- Song title placement: bottom third, left-aligned
- No photographic elements — graphic/abstract only
- Each seed family shares a color anchor (e.g., all Time Machines variants share a palette)

---

## Social Producer

**Output:** Preview cards, share images, promotional pieces.

**Resolution:** 1200x630px (Open Graph standard). Secondary: 1080x1080 (Instagram square).

**Style:** Adapts from whichever artist persona fits the content. Adds minimal text overlay — title only, no descriptions.

**Consistency rules:**
- DevCo Band wordmark in bottom-right corner, 10% opacity
- Same typeface across all social pieces
- Must work on both light and dark backgrounds
