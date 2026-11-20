---
title: "Mermaid & PlantUML Diagrams: user guide"
description: Install Mermaid & PlantUML Diagrams, insert and edit diagrams, export to PDF and Word, paste links and convert code blocks.
---

Mermaid & PlantUML Diagrams turns Mermaid and PlantUML text into diagrams on Confluence Cloud pages, with
sharp images in PDF and Word exports. Diagrams are drawn in the browser; the app runs on Atlassian Forge.

## Requirements

- Confluence Cloud.
- A Confluence administrator to install the app.

## Install

1. A Confluence administrator installs the app from the Atlassian Marketplace (when the listing is published).
2. Open a Confluence page in edit mode and insert the **Mermaid & PlantUML Diagrams** macro.

If the site's license is inactive, diagrams are not drawn: the page shows a short notice and the diagram text
in a collapsible block, so no content is lost. Editing, saving and converting stay disabled until the license
is renewed.

## Insert a diagram

1. In the page editor, insert the macro.
2. Write or paste Mermaid or PlantUML text, or open the full-screen editor.
3. The engine is detected automatically: `@startuml`, `@startmindmap` and similar mean PlantUML; otherwise
   Mermaid. You can also choose the engine by hand.
4. Save the diagram from the editor so that export images are stored.

### Full-screen editor

The editor offers line numbers, a live preview next to the text, and samples for common diagram types
(flowchart, sequence, class, state, ER, Gantt, mind map, timeline; PlantUML sequence, class, activity,
component). You can Save without closing the editor.

### View, zoom and download

On the published page you can open a full-screen view with zoom, pan, fit and reset; download the diagram as
SVG or high-resolution PNG; and copy the diagram text. The app follows the Confluence light or dark theme.
Toolbar buttons have labels and are reachable with the keyboard. Diagram text is indexed by Confluence search.

## Supported diagrams

**Mermaid 12:** flowchart, sequence, class, state, entity relationship, Gantt, pie, mind map, timeline, user
journey, git graph, quadrant, C4, architecture, XY chart, Sankey, block, kanban, and ELK layout.

**PlantUML:** sequence, use case, class, activity, component, state, object, deployment, timing, Gantt, mind
map, WBS, salt (wireframes), JSON, YAML, and more. PlantUML uses its built-in Smetana layout engine, which
runs in the browser.

## Sharp exports

When a diagram is saved in the editor, the app keeps an SVG and a high-resolution PNG (2×) of it. PDF and Word
exports of the page use that PNG, at the diagram's normal size.

- A diagram that was never saved in the editor is drawn live in PDF exports and appears as its source text in
  Word exports.
- After a diagram's text is changed outside the editor, open and save it once to refresh the export image.
- Confluence's Word export is a `.doc` file made for Microsoft Word. LibreOffice and some other editors show
  it as raw code: see [Troubleshooting](#troubleshooting).

## Paste a link

Pasting a mermaid.live or plantuml.com link on a page creates the macro. The diagram is decoded inside the
browser; the app makes no request to those sites.

## Convert existing code blocks

From the page menu, choose **Apps → Convert code blocks to diagrams**. The app lists the `mermaid` and
`plantuml` code blocks of the page (also inside expands and tables). Selected blocks are turned into
diagrams. The change is saved as a new page version made by the user.

## Limits

- Diagram text: a warning above 200 KB; saving is blocked above 1 MB.
- PlantUML: Graphviz-based layouts and remote `!include` are not available. The C4 standard library for
  PlantUML is not included. `nwdiag` diagrams are not supported. Mermaid's C4 diagrams are available.
- Very large pages with dozens of diagrams take a few seconds to draw everything.

## Troubleshooting

- **Diagram looks wrong after an export or after editing outside the editor:** open the diagram in the
  full-screen editor and Save once to refresh the stored PNG.
- **Paste of a mermaid.live or plantuml.com link did nothing:** paste on the page in edit mode; the link is
  decoded in the browser with no call to those sites.
- **Convert did not find a block:** check that the code block language is `mermaid` or `plantuml`, including
  blocks inside expands and tables.
- **License notice instead of a diagram:** renew the Marketplace license; content is kept in a collapsible
  block until then.
- **The Word export opens as code** (lines such as `Content-Type:` and `<html>`): Confluence exports to Word
  as a web page saved with a `.doc` extension, which Microsoft Word opens as a document. LibreOffice and some
  other editors cannot read this format. Open the file in Microsoft Word, or export the page to PDF instead.
  This happens with any Confluence page, with or without diagrams.

If the problem remains, see [Support](https://steadyseam.com/support.html#mermaid-plantuml-diagrams).

## Data, privacy and security

- The app runs entirely on Atlassian Forge. Diagrams are drawn in the user's browser. Steadyseam has no
  servers of its own and does not receive or see your data.
- Diagram text is stored by Confluence in the macro on the page. SVG and PNG images of saved diagrams are kept
  in the app's Forge key-value storage on your site, hosted by Atlassian, with the data residency of the site.
- The app declares no external domains and does not contact any service outside Atlassian. It is eligible for
  Atlassian's "Runs on Atlassian" program.
- No usage analytics and no tracking.

Details: [privacy policy](privacy-policy.md), [Data Processing Addendum](dpa.md), [security](security.md).

## Uninstalling

When the app is uninstalled, Atlassian deletes the data stored by the app according to its data retention
policy for Forge apps. Diagram text that remains in Confluence page content is unchanged.
