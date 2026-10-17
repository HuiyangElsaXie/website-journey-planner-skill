# Website structure and journey plan

## Brief
Lantern Thread is a fictional scarf shop on Shopify. The audience is people already considering a scarf; the goal is a completed purchase (F1). Lifecycle, acquisition source and site language are unknown. This plan uses English provisionally and preserves supplied URLs. Only the owner inventory and brief were inspected; no site, crawl, screenshots, analytics, rendered appearance, mobile usability, speed or live purchase behavior was inspected (F3).

## Evidence ledger
| ID | Fact or observation | Source and date | Confidence / limits |
|---|---|---|---|
| F1 | Shop: Lantern Thread; platform: Shopify; audience: people considering a scarf; goal: purchase | Supplied brief, comparison date 2026-10-17 | Owner-supplied fictional context; platform does not establish purchase controls or routes |
| F2 | Inventory contains /scarves (collection), /scarves/linen-scarf (product description), /contact (contact information) | I1 owner inventory, 2026-10-17 | Supplied inventory only; pages and links not independently inspected |
| F3 | No crawl, analytics, screenshots, link/button labels, cart URL, checkout route, actor-specific permissions or actual purchase sequence supplied | Supplied brief and I1, 2026-10-17 | These remain unknown |
| F4 | A visitor can buy the scarf; owner requests a clear route and compact page-role table | I2 owner brief, supplied for comparison 2026-10-17 | Purchase capability asserted; exact process unknown |

## Current state
Reusable supplied inventory only:

| Current URL | Supplied purpose | Audience | Existing inbound / next-step links |
|---|---|---|---|
| /scarves | Collection | Not specified per page | Unknown |
| /scarves/linen-scarf | Product description | Not specified per page | Unknown |
| /contact | Contact information | Not specified per page | Unknown |

Source: F2. Site-level audience is known (F1), but page-specific intent is not supplied. Current navigation, purchase controls, permissions and routes are unknown (F3). No cart, checkout, homepage or confirmation page is part of the supplied inventory.

## Proposed architecture
Proposal: retain all three supplied URLs and connect collection discovery to product evaluation, with contact available for unresolved questions. No placeholder pages are needed for this lightweight plan. The indentation below is a proposed navigation relationship, not evidence of existing links or a complete site crawl.

- /scarves — collection
  - /scarves/linen-scarf — product description
- /contact — support information
- Purchase destination — unknown; resolve before specifying a URL or adding it to inventory

| Page / URL | Existing or proposed | Audience question | Proposed key content | Proposed next action | Evidence / rationale |
|---|---|---|---|---|---|
| /scarves | Supplied page; proposed role | Which scarf should I consider? | Clear collection choices using verified product information | Link to /scarves/linen-scarf; proposed label: “View linen scarf” | F2; makes the supplied product discoverable |
| /scarves/linen-scarf | Supplied page; proposed role | Is this scarf right for me, and how do I purchase it? | Verified product details plus purchase-relevant availability, delivery and returns information where confirmed; all such details are currently unprovided | Verified purchase control/destination, currently unknown; proposed wording subject to actual action: “Buy this scarf” | F1, F2, F4; supports evaluation and purchase without inventing product facts |
| /contact | Supplied page; proposed role | How can I resolve a question before buying? | Owner-confirmed contact information | Use the verified contact method; method and existing label unknown | F2; recovery route for unanswered questions |

## Proposed navigation and links
Proposal: header link “Scarves” to /scarves and “Contact” to /contact; footer repeats the contact link. Proposed contextual links connect collection to product and product to contact, with a return link to /scarves. These labels and links are drafts, not observed controls (F3).

Preserve every supplied URL; no redirect or old-to-new mapping is proposed. Orphan and duplicate-page status cannot be assessed from an inventory without links. Within the proposed structure, each supplied page has a discoverable route and a distinct role.

## Proposed ready-to-act journey
| Audience / intent | Entry and evidence status | Page sequence: known / proposed / assumed per step | Decision / CTA destination and label status | Success signal | Friction hypothesis | Alternative / recovery |
|---|---|---|---|---|---|---|
| Person already considering a scarf; ready to purchase (F1). Exact actor permissions unknown (F3) | Proposed entry: /scarves; entry source unknown. Direct entry to product is an alternative, not observed behavior | 1. /scarves: supplied page, proposed entry. 2. /scarves/linen-scarf: supplied page, proposed link from collection; existing link/label unknown. 3. Purchase action and any intervening steps: unknown, unverified; no cart or checkout sequence asserted. 4. Completion state: unknown, unverified | Decide whether the scarf fits their needs. Proposed collection CTA “View linen scarf” points to supplied product URL. Current purchase button label, permissions and destination unknown; proposed purchase wording “Buy this scarf” requires verification against actual behavior | Target: an order is completed. Customer-facing confirmation and any measurable event are unknown; no success has been observed | Hypothesis: missing product or purchase information could interrupt the decision; no usability defect or conversion impact established | Proposed direct product entry skips collection. Proposed /contact route resolves questions; failed purchase behavior and recovery controls remain unknown and must be verified |

## Priorities and validation
| Proposal | Rationale and evidence | Effort / constraint | Validation / owner decision |
|---|---|---|---|
| First: document the actual purchase path and controls | F3 leaves the steps supporting F4 unknown | Short owner walkthrough; no site change required | Confirm each actor, label, destination, intervening step and completion/failure state |
| Then: connect collection, product and contact as proposed | Supports the task in F1 using the inventory in F2 | Effort unknown until current links are documented | Compare proposed links with current links before deciding any changes |
| Then: review product-page decision information | Purchase goal in F1; detail completeness uninspected | Content effort depends on available verified facts | Owner supplies accurate product and purchasing information; omit unsupported claims |

## Open questions
Material missing evidence: actual purchase sequence, actor permissions, current labels and destinations, current navigation, product decision information, completion and failure/recovery behavior. Acquisition source and lifecycle are also unknown. No baseline, uplift, prices, stock, guarantees or customer research are assumed.

Next verification step: ask the owner for one annotated ready-to-buy walkthrough starting at /scarves/linen-scarf, recording each actual actor, button/link label, destination, intervening step and confirmation or failure state. Use it to replace unknown journey cells before handing the route to implementation.

Implementation status: Plan only; no live changes.
