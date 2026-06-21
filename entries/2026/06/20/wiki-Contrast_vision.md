---
source: sources/wiki-Contrast_vision.md
source_url: https://en.wikipedia.org/wiki/Contrast_(vision)
---

## Visual Contrast: Definitions, Quantification, and Sensitivity

This page covers the concept of contrast in human vision and imaging — how differences in luminance or color make objects distinguishable from backgrounds. It details the biological basis of contrast sensitivity, formal mathematical definitions for quantifying contrast (Weber, Michelson, RMS), contrast sensitivity functions and their clinical significance, and contrast threshold research.

## Key Concepts

- **Contrast** is the difference in luminance or color that makes an object distinguishable from its background.
- Human vision is sensitive to **relative** luminance differences, not absolute luminance — perceived appearance stays stable despite large illumination changes (Weber–Fechner law).
- **Contrast ratio / dynamic range**: the maximum contrast an image can display. In high-contrast-ratio images, increasing contrast in one region necessarily decreases it elsewhere (*conservation of contrast*).
- **Contrast sensitivity function (CSF)**: the human CSF has a **band-pass filter** shape, peaking at ~4 cycles per degree (cpd), dropping at both higher and lower frequencies.
- **High-frequency cutoff** (~60 cpd): limited by the optical resolution of the eye and photoreceptor packing density in the retina.
- **Low-frequency drop-off**: caused by **lateral inhibition** in retinal ganglion cells, which have center-surround receptive fields.
- **Contrast sensitivity** peaks around age 20 at 2–5 cpd; it declines with age, cataracts, diabetic retinopathy, and neurological conditions.
- **Contrast threshold**: the minimum contrast detectable; contrast sensitivity = 1 / contrast threshold.
- Visual acuity (Snellen chart) tests at 100% contrast and does not capture contrast sensitivity deficits — a patient can have 20/20 acuity yet poor contrast sensitivity.

## Commands and Syntax

**Weber Contrast** — used for small features on a large uniform background:

```
C_Weber = (I - I_b) / I_b
```
- `I` = feature luminance, `I_b` = background luminance

**Michelson Contrast** — used for periodic patterns (sine-wave gratings) where bright and dark areas are equally represented:

```
C_Michelson = (I_max - I_min) / (I_max + I_min)
```
- Range: 0 (no contrast) to 1 (maximum contrast)
- Also called **visibility** or **modulation**

**RMS Contrast** — independent of spatial frequency; standard deviation of pixel intensities:

```
C_RMS = sqrt( (1/MN) * ΣΣ (I_ij - Ī)² )
```
- Pixel intensities normalized to [0, 1]; equivalent to σ/μ of pixel values

**Clinical test charts**: Pelli-Robson (uniform-size letters, decreasing contrast), Regan chart, Arden grating chart, Campbell-Robson chart.

## Relationships

- **Weber–Fechner Law**: underpins why contrast is expressed as a ratio (luminance difference / average luminance) — small differences matter more at low luminance.
- **Spatial frequency**: contrast sensitivity is frequency-dependent; the CSF relates contrast perception to spatial frequency in cpd.
- **Ricco's Law**: Crumey's threshold model is based on an underlying linearity related to Ricco's law (spatial summation for small stimuli).
- **Visual acuity**: complementary to contrast sensitivity — acuity measures resolution at maximum contrast; CSF measures sensitivity across contrast levels.
- **Retinal physiology**: center-surround receptive fields of ganglion cells explain the band-pass shape of the CSF (lateral inhibition causes low-frequency attenuation).
- **Scotopic vs. photopic vision**: contrast thresholds differ between rod-mediated (scotopic) and cone-mediated (photopic) vision, modeled separately by Hecht's formula.
- **Light pollution / astronomy**: Crumey's generalized threshold model applies contrast sensitivity to naked-eye and telescopic stellar visibility.

## Exam-Relevant Points

- The human CSF peaks at **~4 cpd** and has a high-frequency cutoff at **~60 cpd** (Campbell & Robson, 1968).
- **Weber contrast** is for small targets on uniform backgrounds; **Michelson contrast** is for periodic patterns with equal bright/dark areas; **RMS contrast** is frequency-independent.
- The low-frequency CSF drop-off is due to **lateral inhibition** (center-surround receptive fields); the high-frequency cutoff is due to **optical resolution limits and photoreceptor density**.
- Contrast sensitivity peaks around **age 20** and declines with age, cataracts, ARMD, glaucoma, amblyopia, stroke, and Alzheimer's disease.
- A patient can have **normal visual acuity (20/20) but impaired contrast sensitivity** — these are independent measures. This explains functional deficits (e.g., night driving difficulty) despite good acuity scores.
- **Blackwell (1946)**: landmark study using forced-choice procedure (90,000 observations, 7 observers); defined threshold as Weber contrast at 50% detection.
- Contrast sensitivity = **1 / contrast threshold** (reciprocal relationship).
- The denominator in Michelson contrast equals **twice the average luminance** of max and min values.
- **Bleach bypass** reduces contrast in extremes while enhancing it in midtones.
