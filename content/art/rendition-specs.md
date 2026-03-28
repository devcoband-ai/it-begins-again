# Rendition Specifications

Technical guidelines for adapting artwork across different uses and platforms.

---

## Master → Chapter Header

**Source:** Full-resolution master (minimum 2048x2048)
**Target:** 16:9 crop at 2560x1440
**Process:**
1. Select focal region — the emotional center of the image, not necessarily the geometric center
2. Crop to 16:9, preserving the focal region in the upper two-thirds (lower third reserved for chapter title overlay in layout)
3. Apply uniform grain layer (match series grain profile)
4. Export as JPG at 95% quality
5. Generate thumbnail at 800x450 for GitHub preview

**Naming:** `chapter-[N]-[slug].jpg` (e.g., `chapter-5-pool-hall.jpg`)

---

## Master → Gallery Piece

**Source:** Full-resolution master
**Target:** 1:1 or 4:5, resolution preserved
**Process:**
1. Crop to target ratio — composition-driven, no mechanical centering
2. Color-correct to series palette (warm midtones, muted highlights)
3. Optional: add border treatment (thin black or off-white, consistent across gallery)
4. Export as PNG (lossless) for gallery display

**Naming:** `[descriptive-slug].jpg` (e.g., `living-geometry-warped.jpg`)

---

## Master → Album Art

**Source:** Full-resolution master or purpose-built from Album Art Template
**Target:** 3000x3000 (1:1 square)
**Process:**
1. If adapting from a non-square master: crop to 1:1 with the visual hook centered
2. Verify legibility at 300x300 (streaming thumbnail test) — if key elements disappear, simplify
3. No text baked into the image — title and artist handled by platform metadata
4. Export as PNG at full resolution; JPG at 95% for repo storage

**Naming:** `[seed-name]-[variant].jpg` (e.g., `rare-radio-take-me-with-you.jpg`)

---

## Master → Social Card

**Source:** Any existing artwork (chapter header, album art, gallery piece)
**Target:** 1200x630 (Open Graph) or 1080x1080 (Instagram)
**Process:**
1. Select or crop source to target ratio
2. Darken edges slightly (vignette) to create space for text overlay
3. Add title text: white, sans-serif, upper-left or center, sized for readability at 600px wide
4. Add DevCo Band wordmark: bottom-right, 10% opacity
5. Export as JPG at 90%

**Naming:** `social-[slug]-[platform].jpg` (e.g., `social-rare-radio-og.jpg`)

---

## Master → Interactive / HTML

**Source:** Concept or master image as visual reference
**Target:** Responsive HTML/CSS/JS file
**Process:**
1. Translate the visual concept into code — geometry, color, motion
2. Match palette to series standards
3. Ensure responsive behavior (scales to viewport)
4. Include static fallback screenshot as `[slug]-fallback.jpg`
5. Keep file self-contained — no external dependencies

**Naming:** `[descriptive-slug].html` (e.g., `living-geometry-radial.html`)

---

## Cross-Rendition Consistency Checklist

Before committing any new artwork rendition:

- [ ] Palette matches series standards (warm earth base, chapter-specific accent)
- [ ] Grain/texture layer is consistent with existing chapter art
- [ ] Reads clearly at target size AND at thumbnail
- [ ] No baked-in text (titles handled in layout/metadata)
- [ ] File naming follows convention
- [ ] Master file preserved — renditions are always derived, never destructive
