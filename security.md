---
title: "Security: Mermaid & PlantUML Diagrams – Sharp Export for Confluence"
description: How Mermaid & PlantUML Diagrams protects your data, the permissions it uses and how to report a vulnerability.
---

**Reporting a vulnerability.** Write to **support@steadyseam.com** with the details; please do not disclose it
publicly before we have answered. We acknowledge reports within two business days and keep you informed until
the issue is fixed.

**Incident response.** We maintain a written incident response plan. For a confirmed security incident we
notify Atlassian within 24 hours and affected customers within 72 hours.

**How the app is built**

- It runs on Atlassian Forge: no servers of ours. Diagrams are drawn in the user's browser. SVG and PNG images
  of saved diagrams are kept in your site's Forge key-value storage, hosted by Atlassian, with the data
  residency of the site. Steadyseam does not receive or see your data.
- **No external network calls.** The app declares no external domains and does not contact any service outside
  Atlassian, including mermaid.live and plantuml.com. It is eligible for Atlassian's "Runs on Atlassian"
  program.
- **Permissions.**
  - `storage:app`: keep the export images;
  - `read:page:confluence`: read the page to find code blocks to convert, and to read a pasted diagram link
    during export;
  - `write:page:confluence`: save converted code blocks, done as the current user;
  - `read:content.permission:confluence`: check that the person saving a diagram's images can edit the page.
- **Security controls.**
  - every SVG is sanitized (scripts, event handlers and unsafe links removed) before it is shown;
  - image saving is refused unless the user can edit the page, and each image is tied to its page and macro;
  - inputs are validated on the server;
  - dependencies are checked with `npm audit` before each release.
- **Content Security Policy.** Only inline styles are allowed (`content.styles: unsafe-inline`), because
  Mermaid styles its diagrams inline. No `unsafe-eval`.
- **Logs** contain event names, sizes, counts and error types, never diagram text or page content.
- No usage analytics, no tracking, no data sent to Steadyseam.

See also the [privacy policy](privacy-policy.md) and the [Data Processing Addendum](dpa.md).
