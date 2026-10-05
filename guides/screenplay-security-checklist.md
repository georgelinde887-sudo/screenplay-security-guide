# Screenplay Security Checklist: Pre-Flight Verification for Film & TV

Before sending an unreleased screenplay, episodic pilot, or pitch treatment to any external party, execute this pre-flight verification checklist. Following these standardized stages minimizes leak vectors, ensures legal traceability, and prevents embarrassing metadata exposure.

---

## Phase 1: Document Sanitization (Local PDF)

Never upload or distribute an uninspected screenplay directly exported from screenwriting software (Final Draft, WriterDuet, Fade In, Highland).

- [ ] **Sanitize Title Page Contact Details**: Remove personal mobile numbers, home addresses, or private email accounts from the title page. Substitute official production office contacts or representation details.
- [ ] **Strip Software Revision Metadata**: Ensure internal writer notes, script editor comments, discarded beat revisions, and track-changes history are purged before PDF generation.
- [ ] **Verify Page Numbering & Format Standard**: Ensure Courier 12pt formatting, standard 1.5" left margin, 1.0" top/bottom/right margins, and sequential page numbering.
- [ ] **Verify Title Consistency**: Ensure the filename does not reveal secret working titles or unannounced cast attachments (e.g., use `PROJECT_CODENAME_DRAFT_2026.pdf`).

---

## Phase 2: Access Gating Configuration

Decouple the file from raw delivery by establishing access prerequisites.

- [ ] **Email Identification Activated**: Verify that viewers must authenticate their email address before accessing page content.
- [ ] **Recipient Whitelisting (For High Stakes)**: If the document is restricted to specific executives or talent, add their exact professional email addresses to the whitelist.
- [ ] **Password Protection Configured**: Set a unique, high-entropy document password.
- [ ] **Out-of-Band Delivery Planned**: Prepare to deliver the password via a separate communication channel (Signal, SMS, phone call) rather than in the same email containing the link.
- [ ] **Direct Downloads Disabled**: Confirm that the "Allow Download" toggle is turned off so the original PDF remains within the secure cloud viewer.
- [ ] **Screenshot Blocker Activated**: Enable browser-level screenshot suppression controls.

---

## Phase 3: Visual Attribution & Legal Gates

Ensure visual and legal deterrence accompany technical access controls.

- [ ] **In-Line NDA / Agreement Gate Enabled**: Paste the production's standard mutual or unilateral confidentiality agreement into the agreement gate drawer.
- [ ] **Dynamic Watermark Configured**:
  - Interpolation syntax active: `{{email}} • {{date}} {{time}}`
  - Layout set to **Tiled (Repeating)**
  - Rotation calibrated to **-30°** or **-45°**
  - Opacity verified between **10% and 14%** (checked for contrast against text)
- [ ] **Studio / Production Logo Applied (Optional)**: If using a custom production logo watermark, verify that it does not clash with the dynamic text overlay.

---

## Phase 4: Link Generation & Distribution

Avoid sending universal public links to multiple competing external entities.

- [ ] **Dedicated Link Slugs Created**: If submitting to three distinct financiers, create three separate links (e.g., `/s/script-producer-a`, `/s/script-producer-b`, `/s/script-financier-c`).
- [ ] **Access Expiration Set**: Define an upfront expiration window (e.g., 7 or 14 days) to prevent stale links from circulating indefinitely.
- [ ] **Test Link in Incognito Window**: Open the generated URL in a private/incognito browser window to verify the user onboarding journey:
  1. Email prompt appears
  2. Password prompt appears
  3. NDA agreement displays clearly
  4. Watermark renders legibly over scene headers

---

## Phase 5: Post-Submission Auditing & Follow-Up

Telemetry should inform your production decisions and creative timeline.

- [ ] **Monitor First-Read Alerts**: Check the dashboard to confirm when the recipient first logs in.
- [ ] **Evaluate Page Dwell Distribution**:
  - Check dwell time on Pages 1–10 to confirm whether the recipient gave the script a genuine read.
  - Review overall completion percentage before scheduling follow-up calls.
- [ ] **Audit NDA Execution Record**: Verify that the recipient's signature, timestamp, and network telemetry are recorded in the session log.
- [ ] **Revoke Stale or Declined Access**: If a party officially passes on the project, immediately deactivate their specific link slug to revoke ongoing access.

---

## Quick Reference Summary Table

| Checklist Phase | Primary Threat Mitigated | Responsible Role |
|---|---|---|
| **Phase 1: Sanitization** | Accidental exposure of personal phone numbers or draft revision notes | Writer / Script Coordinator |
| **Phase 2: Access Gating** | Uncontrolled forwarding and unmonitored link distribution | Producer / Production Coordinator |
| **Phase 3: Watermarking & NDA** | Unauthorized screenshot leaks and lack of legal recourse | Production Legal / Producer |
| **Phase 4: Dedicated Links** | Inability to selectively revoke access or isolate telemetry | Producer / Development Assistant |
| **Phase 5: Telemetry Auditing** | Guesswork during packaging and stale link accumulation | Development Executive / Producer |

---

## Related Reading

- [Protecting Screenplay PDFs](protecting-screenplay-pdfs.md) — Architectural overview.
- [Controlled Script Sharing](controlled-script-sharing.md) — Workflow execution across roles.
- [NDA Access for Screenplays](nda-access-for-screenplays.md) — Digital agreement implementation.
- [Screenplay Watermarking](screenplay-watermarking.md) — Visual deterrence design.
- [Screenplay Reader Analytics](screenplay-reader-analytics.md) — Reading telemetry analysis.
