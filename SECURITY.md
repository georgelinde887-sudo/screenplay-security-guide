---
layout: default
title: "Security Policy and Disclosure Guidelines"
description: "Security policy, realistic digital rights management boundaries, and responsible disclosure procedures for screenplay security."
canonical_url: "https://georgelinde887-sudo.github.io/screenplay-security-guide/SECURITY.html"
---

# Security Policy and Disclosure Guidelines

The **Screenplay Security Guide** aims to provide realistic, technically rigorous information regarding document security, controlled access, and leak deterrence for the film and television industry.

---

## Technical Security Boundaries & Honest Expectations

When distributing confidential scripts and production documents, understanding security boundaries is critical:

1. **Client-Side Display Realities**: Any document displayed on a remote device must ultimately be decoded into memory and rendered on a screen. While access gates, dynamic watermarks, and browser controls deter casual distribution, no browser-based technology can prevent an authorized viewer from taking a physical photo of their screen with an external smartphone.
2. **Watermarking as Traceability, Not DRM**: Dynamic watermarks do not physically prevent capture; they bind the recipient's identity (email, timestamp, IP hash) to the visual rendering so that leaked pages can be attributed to the originating session.
3. **Defense in Depth**: Robust screenplay security relies on a layered combination of:
   - Identity verification (email OTP or verified session)
   - Access restriction (passwords and domain/email whitelisting)
   - Legal deterrence (in-line NDA acknowledgement prior to view)
   - Visual attribution (dynamic and custom watermarks)
   - Download prevention (streaming/canvas rendering rather than raw PDF download)
   - Telemetry (session duration and page-level engagement tracking)

---

## Reporting Vulnerabilities or Documentation Flaws

If you discover a security flaw in any sample script, automated script, or find technical inaccuracies that misrepresent digital rights management boundaries:

- Please open an issue or reach out to the repository maintainers via GitHub.
- For issues concerning third-party platforms mentioned in implementation examples (such as SendNow), please contact the platform's security team directly at their official security contact: [security@sendnow.live](mailto:security@sendnow.live).
- When reporting documentation discrepancies, please specify the exact file path, the claim made, and the empirical or technical standard that contradicts it.
