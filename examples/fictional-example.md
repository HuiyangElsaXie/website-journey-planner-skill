# Fictional example: Lantern Workshop

This is a completely fictional business, brief and page excerpt created to demonstrate the workflow. It is not a client case study or measured result. / 完全虚构的业务与材料，仅用于展示使用方式，不代表客户案例或已验证成效。

## Brief and evidence
- F1: Fictional supplied brief, dated 2026-10-16: Lantern Workshop offers beginner paper-craft workshops. Audience: adults looking for a first workshop. Goal: receive relevant enquiries. Lifecycle: pre-launch.
- F2: Fictional supplied inventory, same date: Home /, Workshops /workshops, About /about, Contact /contact. Contact page invites an enquiry. No analytics or rendered pages supplied.
- F3: Fictional constraint, same brief: keep existing URLs; one person maintains the site. Dates, prices, available places and booking terms are not supplied.
- Scope: text/inventory planning only. Actual link behavior, mobile layout and demand are unknown.

## Current state
Four pages are known. Their links and detailed content are unknown. No claim is made that the current site has broken navigation.

## Proposed architecture
- Home /
  - Workshops /workshops
  - About /about
  - Contact /contact

| Page | Audience question | Proposed content | Next action |
|---|---|---|---|
| Home | Is this relevant to a beginner? | Brief introduction supported by F1 | View workshops |
| Workshops | What should I know before enquiring? | Outline plus clearly unresolved dates, prices and materials questions | Ask about a workshop, linking to /contact |
| About | Who runs this? | Owner-approved introduction, requiring source material | View workshops |
| Contact | How do I enquire? | Existing enquiry route from F2; exact form fields unknown | Send enquiry, behavior to verify |

Header proposal: Workshops, About, Contact; logo links home. Footer: repeat relevant contact information only when supplied. Add a contextual Workshops → Contact link. Preserve all four URLs; no redirect proposed. No orphan-page finding can be asserted from the inventory alone.

## Proposed journeys
1. Still researching: referral → Home → Workshops → About → Workshops. Decision: whether the workshop fits. Success signal proposal: visitor finds the suitability information. Recovery: ask a question on Contact when details are missing.
2. Ready to enquire: direct Workshops entry → Contact → existing confirmation state, currently unverified. Decision: send an enquiry. Success signal proposal: enquiry accepted, not merely a button click. Recovery: clear form error and alternate contact route if available, both requiring implementation review.

## Priorities and validation
- First: confirm workshop essentials before drafting promises. F3 leaves key purchase questions unanswered.
- Next: review the two journeys using a paper walk-through. Ask a reviewer where they would find beginner suitability and how to enquire.
- Then: verify the actual enquiry destination and confirmation/error states in a separately authorized implementation review.

No conversion baseline or uplift is asserted. These are proposals. No live changes were made.

