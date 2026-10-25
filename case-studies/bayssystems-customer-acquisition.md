# BaysSystems Customer Acquisition

A technical case study of an internal email acquisition system built around human approval, queued delivery, and reply tracking.

## Business problem

Prepare relevant outreach drafts, review them before delivery, track replies, and stop unnecessary follow-ups without losing processing history.

## My contribution

Business workflow design, AI-assisted implementation, integration, and delivery verification.

## Workflow

Imported business records → draft preparation → human review → approved queue → dry-run delivery.

Reply handling associates incoming messages with a business record, cancels follow-ups, and prevents duplicate processing.

## Implementation

- Application service with PostgreSQL and Docker Compose
- Human review interface and delivery queue
- SMTP delivery and IMAP reply handling
- n8n operational notifications
- Duplicate-message protection
- Backup and recovery procedures

## Verification status

Development reports recorded 78 passing tests and a successful mock end-to-end chain. Controlled email tests showed SPF, DKIM, and DMARC passing. A real incoming reply was used to check matching, follow-up cancellation, and duplicate protection in an isolated test database.

These are reported development checks, not an independently repeated audit.

## Current status

The campaign remains disabled. The default workflow uses mock providers and dry-run mode. Real AI output quality, automated business discovery, brochure integration, and commercial launch checks remain pending.

This case study demonstrates implementation and controlled testing. It does not claim paying clients or measured acquisition results.

## Public scope

Application source, credentials, contact records, and infrastructure identifiers are not included.
