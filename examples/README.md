---
layout: default
title: "Demonstration Screenplay: THE LAST CUT Test Payload"
description: "Testing protocols and benchmark verification procedures using the fictional sample screenplay THE LAST CUT."
canonical_url: "https://georgelinde887-sudo.github.io/screenplay-security-guide/examples/"
---

# Fictional Demonstration Screenplay: "THE LAST CUT"

This directory contains a sample screenplay document used throughout this repository to illustrate secure document workflows, viewer access gating, watermark positioning, and engagement analytics.

---

## Document Details

- **File**: [`sample-screenplay.pdf`](./sample-screenplay.pdf)
- **Title**: *THE LAST CUT*
- **Format**: Standard 5-page industry screenplay format (Courier 12pt, standard margins and scene headings)
- **Nature of Content**: **Fictional sample screenplay created strictly for demonstration purposes.**
  - This document is **not** an excerpt from a real production.
  - It is **not** based on any existing motion picture, television project, or third-party intellectual property.
  - It is provided solely as a benign test payload for testing document access controls, dynamic watermarking, and reader telemetry.

---

## How to Use This Sample for Workflow Testing

When evaluating a secure sharing platform (such as [SendNow](https://sendnow.live/) or an internal virtual data room), use this sample file to verify your security configuration before sharing real, confidential studio drafts:

1. **Test Watermark Readability**:
   - Upload `sample-screenplay.pdf` to your sharing platform.
   - Configure a dynamic watermark string: `{{email}} • {{date}} {{time}}`.
   - Set the opacity to ~12% and rotation to -30°.
   - Inspect page 1 and page 2 to verify that scene headers (`INT. EDIT SUITE - NIGHT`) and character dialogue remain clearly readable while the watermark visibly covers text blocks.
2. **Verify Mobile Viewing Performance**:
   - Open the resulting secure link on mobile devices (iOS Safari, Android Chrome).
   - Ensure that viewport scaling does not clip dialogue margins or introduce horizontal scroll bars.
3. **Audit Access Gating**:
   - Enable email gating, password protection, and the in-line NDA gate.
   - Open an incognito browser tab and verify that the script content is completely blocked until all three gates are successfully completed.
4. **Inspect Telemetry Logging**:
   - Read pages 1 and 2, pause for 15 seconds, and then close the tab without scrolling to page 5.
   - In your sender analytics dashboard, confirm that page-by-page dwell time accurately reflects engagement on pages 1–2 with 0s dwell time recorded for unread pages.

---

## Licensing Terms

*THE LAST CUT* is provided under the [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/) license. You may use it freely to benchmark and demonstrate document security systems, but you may not produce, adapt, or commercially exploit the underlying script text.
