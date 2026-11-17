---
title: Mermaid & PlantUML Diagrams – Sharp Export for Confluence
description: Turn Mermaid and PlantUML text into sharp diagrams on Confluence Cloud pages, including PDF and Word exports.
---

![Mermaid & PlantUML Diagrams logo](assets/logo-144.png)

An Atlassian Forge app for **Confluence Cloud** that turns diagrams written as text in Mermaid or PlantUML
into diagrams on the page, with sharp images in PDF and Word exports.

- **One macro for Mermaid and PlantUML.** Insert the macro, write or paste the diagram text. The engine is
  detected automatically (`@startuml`, `@startmindmap` and similar mean PlantUML; otherwise Mermaid), or you
  can choose it by hand.
- **Full-screen editor with live preview.** Line numbers, preview next to the text, samples for common
  diagram types, and Save without closing the editor.
- **Sharp exports.** When you save a diagram in the editor, the app keeps an SVG and a high-resolution PNG
  (2×). PDF and Word exports of the page use that PNG at the diagram's normal size.
- **Fast pages.** Diagrams are drawn only when they become visible, and the saved SVG is shown right away when
  the text has not changed.
- **Full screen, zoom and download.** Zoom, pan, fit and reset; download as SVG or high-resolution PNG; copy
  the diagram text.
- **Paste a link or convert code blocks.** Pasting a mermaid.live or plantuml.com link creates the macro
  (decoded in the browser, with no request to those sites). A page menu action turns selected `mermaid` and
  `plantuml` code blocks into diagrams.
- **No servers of ours.** The app runs on Atlassian Forge. Diagrams are drawn in the user's browser. The app
  declares no external domains and is eligible for Atlassian's "Runs on Atlassian" program.

Submitted to the Atlassian Marketplace (under review), priced per user, free for up to 10 users, with a
30-day free trial for larger sites.

## Demo (about 2 minutes)

<video controls preload="none" poster="assets/demo-poster.jpg" width="100%">
  <source src="assets/demo.mp4" type="video/mp4">
</video>

## Documentation

- [User guide](user-guide.md): installation, editor, exports, paste and convert, limits, data and privacy.
- [Support](https://steadyseam.com/support.html#mermaid-plantuml-diagrams)
- [Privacy policy](privacy-policy.md), [Data Processing Addendum](dpa.md), [Terms](terms.md),
  [Security](security.md), [Third-party licenses](licenses.md)
