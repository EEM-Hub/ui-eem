---
source: sources/wiki-Material_Design.md
source_url: https://en.wikipedia.org/wiki/Material_Design
---

## Google Material Design: Design Language Overview

Material Design is a design language developed by Google, first announced at Google I/O on June 25, 2014 (codenamed "Quantum Paper"). It provides a unified visual system for building user interfaces across Android, iOS, and web platforms. Rooted in the metaphor of paper and ink, it uses grid-based layouts, responsive animations, depth effects (lighting and shadows), and physical-surface semantics to create consistent, intuitive UIs. The language has evolved through three major versions, with the latest being Material 3 Expressive (2025).

## Key Concepts

- **Design metaphor**: Based on paper-and-ink and skeuomorphic principles — "digital material expands and reforms intelligently" with physical surfaces, edges, seams, and shadows
- **Core UI elements**: Grid-based layouts, responsive animations and transitions, padding, depth effects (lighting/shadows), cards UI (originated from Google Now)
- **Head designer**: Matias Duarte led the design effort
- **Three major versions**:
  - **Material Design 1** (2014): Original release with foundational principles
  - **Material Design 2** (2018): Focus on customization, white space, rounded corners, colorful icons, bottom navigation bars; introduced Google Sans font
  - **Material Design 3 / Material You** (2021): Dynamic theming from user wallpaper, increased animation, larger buttons, custom UI theme generation
  - **Material 3 Expressive** (2025): Improved animations, more colorful/fun design; targets Android 16 and Wear OS 6
- **Open source**: Licensed under Apache-2.0 (Android/iOS), BSD-3-Clause (Flutter), MIT (Web)
- **Platform support**: Android (actively maintained), iOS (discontinued), Web (discontinued); Flutter and Jetpack Compose are current recommended implementation paths
- **Dynamic Color**: Material You (MD3) introduced wallpaper-based automatic theme generation on Android 12+

## Commands and Syntax

No CLI commands — Material Design is a design specification, not a CLI tool. Implementation is through libraries:

- **Android (Jetpack Compose)**: `material-components-android` — latest stable 1.12.0 (May 2024)
- **Flutter**: `material-components-flutter` — canonical cross-platform implementation
- **Web**: `material-components-web` (Material Web) — canonical web implementation, v14.0.0 (April 2022, discontinued as standalone)
- **iOS**: `material-components-ios` — v124.2.0 (April 2021, discontinued)

Official implementation guidance available at:
- m3.material.io (Material Design 3 / current)
- m2.material.io (Material Design 2 / archived)
- m1.material.io (Material Design 1 / archived)

## Relationships

- **Android ecosystem**: Material Design is the official design language for Android; tightly integrated with Android releases (Lollipop, Pie, Android 12, Android 16)
- **Flutter**: Primary cross-platform framework for implementing Material Design; Material widgets are built into Flutter's core
- **Jetpack Compose**: Android's modern declarative UI toolkit with native Material 3 support
- **Competing design systems**: Flat Design, Microsoft's Fluent Design System, Apple's Human Interface Guidelines, Metro (Microsoft), Corporate Memphis, Apple's Liquid Glass
- **Google products**: Rolled out across Gmail, Calendar, Docs, Google Photos, Google Contacts, and all major Google apps
- **Pixel devices**: Material You was a major focus of Pixel 6 series; Material 3 Expressive rolled out to Pixel 6+ devices starting September 2025

## Exam-Relevant Points

- Material Design was announced at **Google I/O 2014** (June 25, 2014) and codenamed **Quantum Paper**
- **Material Design 2** (2018) appeared with **Android Pie** and emphasized **customization** and **white space**
- **Material You / Material Design 3** (2021) launched with **Android 12** and introduced **dynamic color theming from wallpaper**
- **Material 3 Expressive** (2025) targets **Android 16** and **Wear OS 6**
- The canonical web implementation is called **Material Web**; Flutter and Jetpack Compose are the primary recommended frameworks
- iOS and standalone Web component libraries have been **discontinued**; Flutter is the cross-platform path forward
- Material Design is **open source** with platform-specific licenses (Apache-2.0, BSD-3-Clause, MIT)
- **Google Sans** is a size-optimized version of the proprietary **Product Sans** font, introduced with Material Design 2
