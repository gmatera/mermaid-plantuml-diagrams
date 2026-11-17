---
title: "Privacy Policy: Mermaid & PlantUML Diagrams – Sharp Export for Confluence"
description: What data Mermaid & PlantUML Diagrams processes, why, where it is kept and for how long.
---

*Last updated: 17 November 2026.*

This policy explains what data the Atlassian Marketplace app **Mermaid & PlantUML Diagrams – Sharp Export for
Confluence** (the "App") processes, why, where it is kept and for how long. The App is provided under the
Steadyseam brand by **Sasso di Matera Giuseppe S.a.s.** (Via Clefi 2, 20146 Milano (MI), Italy, VAT
IT13043470965), "we" in this policy. Contact: **support@steadyseam.com**.

## 1. How the App works

The App turns Mermaid and PlantUML diagram text into diagrams on Confluence Cloud pages and keeps sharp images
for PDF and Word exports. It runs on Atlassian's Forge platform and has no servers of its own: we do not
receive or see the data it stores. Diagrams are drawn in the user's browser. The App declares no external
domains and does not contact any service outside Atlassian.

## 2. Data processed by the App

| Data | Source | Purpose |
|---|---|---|
| Diagram text (Mermaid or PlantUML source) | your users, in the page macro | Show and edit diagrams; indexed by Confluence search |
| SVG and high-resolution PNG of each diagram saved in the editor | the App, from the diagram text | Fast display and sharp PDF/Word exports |
| Forge logs: event names, sizes, counts and error types (never diagram text or page content) | the App | Operation and support of the App |

The App does not store Atlassian account IDs, names or e-mail addresses. Diagrams may contain whatever your
organization's users write in them; that content stays within Atlassian.

## 3. Where the data is stored and who receives it

- Diagram text is stored by **Confluence** in the macro on the page, like any other page content.
- SVG and PNG images of saved diagrams are kept in the App's **Forge key-value storage on your site**, hosted
  by Atlassian, with the data residency of the site. When a diagram changes, its previous images are deleted.
- The App does not send data to us. Atlassian is our only sub-processor (see the
  [Atlassian Privacy Policy](https://www.atlassian.com/legal/privacy-policy)).

## 4. Retention

- Diagram text: for as long as it remains in the Confluence page (controlled by your organization).
- Export images (SVG and PNG): until the diagram is changed (previous images are deleted) or the App is
  uninstalled.
- When the App is uninstalled, Atlassian deletes the data stored by the App according to its data retention
  policy for Forge apps.

## 5. Logs and tracking

The App's technical logs contain event names, sizes, counts and error types, never diagram text or page
content. Atlassian lets us see them only within the limits it sets. The App uses no usage analytics and no
tracking, and sends no data to Steadyseam.

## 6. Roles and your rights

For the data listed in section 2, your organization is the controller and we act as a processor on its
behalf, under our [Data Processing Addendum](dpa.md). Requests from people whose data appears in diagram text
should be addressed to your organization, which can change or delete that content in Confluence; we will
assist on request.

When you contact our support, we use your name, e-mail address and the content of your message only to answer
you, and we keep them for up to 24 months after the last exchange. You can ask us to access, correct or delete
them, or object to their use, by writing to support@steadyseam.com. You can also lodge a complaint with your
data protection authority (in Italy, the Garante per la protezione dei dati personali).

## 7. Security

Every SVG is sanitized before it is shown. Image saving is refused unless the user can edit the page, and each
image is tied to its page and macro. Inputs are validated on the server. See the
[security page](security.md).

## 8. Changes

We will publish any change to this policy on this page, with the date of the last update.
