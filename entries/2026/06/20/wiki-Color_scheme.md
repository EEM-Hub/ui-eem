---
source: sources/wiki-Color_scheme.md
source_url: https://en.wikipedia.org/wiki/Color_scheme
---

## Color Schemes in Color Theory

This page covers the taxonomy of color schemes — systematic combinations of two or more colors used in design. It spans aesthetic/harmonious schemes (based on color wheel relationships), practical schemes (optimizing contrast for functional purposes), qualitative schemes (encoding categorical data), quantitative schemes (representing ordered data in visualizations), and connotative schemes (leveraging cultural color associations).

## Key Concepts

- A **color scheme** is a combination of 2+ colors used for aesthetic or practical purposes, typically described by positions on a color wheel or within a color space.
- **Achromatic** colors lack chromatic content (black, white, grays, beiges); **neutrals** are obtained by mixing pure colors with white/black/gray or by mixing two complementary colors.
- **Monochromatic** schemes use tints, tones, and shades of a single hue — subtle and peaceful due to lack of hue contrast.
- **Complementary** colors sit opposite on the color wheel and combine to form gray; they maximize color contrast.
- **Split-complementary** uses a base color plus two colors at 150° and 210° from it — similar contrast to complementary but less visual tension.
- **Analogous** colors are adjacent on the color wheel (typically base ± 30°); they share consistent color temperature but lack contrast.
- **Near-analogous** widens the spread (base ± 60°), adding more contrast while keeping consistency.
- **Accented analogous** adds the complement of one analogous color as an accent.
- **Triadic** = 3 colors at 120° intervals; balanced contrast and richness.
- **Tetradic** (double complementary) = 4 colors in two complementary pairs; hard to harmonize without one dominant color.
  - **Rectangle** variant: base + colors at 60°, 180°, 240°.
  - **Square** variant: base + colors at 90° intervals.
- **Hexadic** = 6 colors at 60° intervals (three complementary pairs / two triadic schemes).
- **Qualitative** schemes encode unordered categorical data; number of colors generally equals number of categories. Color difference matters more than harmony.
- **Quantitative** schemes (color maps) encode ordered data; can be continuous (smooth gradient) or discrete (distinguishable steps).
- **Sequential** schemes: gradient from minimum to maximum value (monochrome, spectral, part-spectral, or scientific variants).
- **Diverging** schemes: two sequential schemes sharing a center color (usually white) representing a meaningful midpoint; darkest values at extremes.
- **Cyclic** schemes: no beginning or end; used for periodic data (angles, wind direction, seasonality).
- **Bivariate/trivariate** schemes blend two or three orthogonal sequential schemes to represent multiple variables simultaneously.
- Humans can see hundreds of shades but only reliably distinguish **5–8** for practical map/legend matching.
- Trade dress law can protect color schemes (e.g., Owens Corning's pink fiberglass).

## Commands and Syntax

No CLI commands; the relevant tools and specifications are:

- **ColorBrewer** (2002, Cynthia Brewer): interactive tool for selecting colorblind-safe, device-reproducible schemes; now a standard in GIS software.
- **Matplotlib (MPL) colormaps**: includes Viridis (default); developed by van der Walt and Smith.
- **Cividis**: colormap optimized for color vision deficiency (Nuñez et al.).
- **CMOcean**: colormaps for oceanographic data (Thyng et al.).
- **CET colormaps**: perceptually uniform (Kovesi).
- **Scientific color maps**: perceptually uniform + colorblind-accessible (Crameri).
- Color wheel degree references for constructing schemes:
  - Complementary: base + 180°
  - Split-complementary: base + 150° + 210°
  - Analogous: base + 30° + 330°
  - Near-analogous: base + 60° + 300°
  - Triadic: base + 120° + 240°
  - Square tetradic: base + 90° + 180° + 270°
  - Rectangle tetradic: base + 60° + 180° + 240°

## Relationships

- **Color wheel / color space**: the spatial framework for defining scheme relationships.
- **Color harmony**: the aesthetic goal of harmonious schemes; quantitative/qualitative schemes may sacrifice harmony for discriminability.
- **Color difference**: critical for qualitative schemes (categorical encoding) and practical schemes (visibility vs. camouflage).
- **Color task taxonomy**: aesthetic tasks (harmonious schemes), comparative tasks (qualitative schemes), connotative tasks (cultural meaning schemes).
- **Data visualization**: quantitative schemes underpin thematic maps, choropleths, heat maps, charts, and spreadsheets.
- **Color blindness / accessibility**: scientifically derived schemes (ColorBrewer, Viridis, Cividis) are designed to be accessible; traditional rainbow/jet schemes are problematic.
- **CIELAB color space**: used by scientific schemes to achieve perceptual uniformity.
- **Trade dress / trademark law**: legal protection for distinctive color schemes in branding.

## Exam-Relevant Points

- Complementary colors are **opposite** on the color wheel (180°); analogous colors are **adjacent** (30°).
- Split-complementary uses 150° and 210° — know the degree offsets for all major schemes.
- Monochromatic = one hue varied by tint/shade/tone; achromatic = no hue at all (black/white/gray).
- Tetradic schemes require a **dominant color** to avoid looking unbalanced.
- Qualitative schemes prioritize **color difference** over harmony; quantitative schemes prioritize **ordered perception**.
- Diverging schemes need a **meaningful center value** (zero, median, parity) represented by a shared neutral color.
- Spectral (rainbow) schemes are **poor for sequential data** because hues don't naturally convey "more" or "less."
- ColorBrewer is the standard reference for **colorblind-safe** map color schemes.
- Practical limit: humans can only distinguish **5–8 shades** in a legend.
- Cyclic schemes have **no endpoints** — used for angular/periodic data.
- The 25-pair color code demonstrates encoding **more categories than colors** by using color pairs (25 values from 10 colors).
