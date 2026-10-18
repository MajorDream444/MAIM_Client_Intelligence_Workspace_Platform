# AMA / MAIM workspace product family
Date: 2026-10-18
Status: proposed product strategy; not a release or validated demand claim.
Owner: Major Dream Williams. Commercial operator: AMA Solutions Corp. Education: MAIM.

## Four entry points
| Experience | Buyer / user | Job | Minimum useful output | Acceptance |
|---|---|---|---|---|
| Readiness Review (proposed Rabbit) | Small advisory team or entrepreneur preparing a decision | Establish what is known and missing | Organized source register, issue list, responsibility map and proceed/revise/stop recommendation | Traceable findings and actionable requests, even when answer is no |
| Client Delivery Workspace | AMA operators, agencies and their clients | Deliver agreed work with clear progress and changes | Scope baseline, milestones, operational/design acceptance, change log | Evidence against agreed criteria and recorded approval |
| Deal Collaboration Workspace (working name AMA DealRoom) | Coordinators working with independent counterparties | Maintain collective context across projects and audiences | Scoped evidence, submissions, revisions, questions and acknowledged contributions | Correct visibility, provenance and reviewable decisions |
| Founder Contribution Lab | MAIM learners and early founder teams | Learn partner alignment before conflict | Synthetic ledger, explicit rules, provisional allocation and reflection | Explain evidence, assumptions, disputes and next decisions; no issued equity |

These are four proposed entry points, not necessarily four standalone software products. A readiness review is a bounded service; the lab begins as education. Delivery and deal collaboration are distinct experiences that may later share proven contracts. Do not force customers through every tier.

## Shared capabilities and boundaries
Candidate shared contracts: workspace identity, membership, server-side permissions, document/version records, evidence links, decisions, audit events, exports and bounded AI assistance. Reuse only after testing fit in both workflows.
Delivery-specific: contractual scope, acceptance, revisions and change approvals.
Deal-specific: unverified claims, authority requests, audience separation and contribution acknowledgment.
Founder-specific: agreed valuation policy, unpaid resources, disputed entries and educational scenarios.
AI proposes tags, summaries and contradictions with citations. People accept findings, access changes, agreements, fees and ownership.
A contribution log is not a cap table, fee entitlement or legal authority. Track stated → evidenced → acknowledged → separately agreed.

## Repository ownership
| Repository | Owns | Does not own |
|---|---|---|
| AMA-Capability-Commercialization-System | Buyer, positioning, offers, price experiments, validation and claim governance | Product runtime or customer records |
| AMA-Rabbit-Delivery-System | Intake, repeatable setup, acceptance, handoff and support playbooks | Marketing truth or private deal archives |
| MAIM_Client_Intelligence_Workspace_Platform | Reusable architecture/contracts, configured experiences and MAIM learning patterns | A specific client's evidence or automatic expansion beyond Stage A |
| HopeKamoaCity_Ports-Project (private) | Actual project instance, archive and scoped review workflows | Universal product doctrine or customer-ready SaaS claims |

Product engineering needs a separately approved code boundary; no new product repository is created by this documentation change. Marine Foundation is the impact-review context of the private instance, not commercial product owner or recipient of commissions under Major's stated arrangement. HAMAL means Hanzo + Art Mob AGInts + Lux. Brand presence alone establishes no commitment.

## Evidence status
Repository READMEs and the platform architecture were read on 18 October. The platform explicitly remains Stage A documentation. The private workspace implementation and tests were reported in the preceding session, not independently re-audited in this update. Customer demand, pricing, SaaS security and repeatability remain Unknown/Requires Verification. Use the commercialization repo's canonical evidence labels and separate provenance from independent verification.

## Commercial sequence and stop rules
1. Days 1–7: Major owns buyer selection; operator interviews five prospective buyers about recent real workflows, existing spend and decision authority. Designer uses synthetic demonstrations. Capture objections and willingness to pilot; no implied purchase.
2. Days 8–14: define one fixed-scope readiness offer and one delivery template. Recruit three to five consented pilots. Operator measures baseline time and setup effort. Engineering documents data/access flows before any live pilot.
3. Days 15–21: deliver pilots with bounded support. Capture first useful result, participant return use, unresolved issues, rework, access failures and support minutes. Seek explicit price feedback; revenue is counted only when actually collected.
4. Days 22–30: review evidence with Major. Proceed to an assisted offer only after operational gates pass. Automate repeated setup after observed repetition, not before. Do not promise self-service subscriptions yet.

Proposed validation thresholds, to confirm before pilots: at least 3/5 complete a useful review; at least 2/5 accept a clearly stated paid next step; median setup <=2 operator hours; support <=30 minutes per room/week; no unresolved access-isolation failure. Report actual denominators. If sample differs, reset thresholds explicitly. If targets fail, narrow the buyer/problem or pause. These are experiments, not forecasts.

Pricing is a hypothesis: test a fixed-fee readiness review, assisted setup plus capped support, and only later room subscriptions with storage/member/AI limits. The MAIM lab can be course-included or cohort-priced after learning validation. Record hosting, storage, AI, setup labor, support, acquisition, refunds and target margin before choosing amounts. Confirm plan limits from providers before committing; free-tier capacity is not a business model.

## Release gates
| Gate | Required evidence / proposed owner |
|---|---|
| Demand | Repeated pain, buyer authority, pilot completion and payment evidence / Major |
| Delivery | Input/output bounds, acceptance, support limits and rollback/handoff / operator |
| Identity and isolation | Verified accounts as needed, per-project and per-tenant negative tests, attachment/export/AI isolation, revocation / engineering |
| Durability | Backups plus restore drill, export, correction, retention/deletion and dependency recovery / engineering |
| Intelligence | Source-linked output evaluation, prompt-injection handling, bounded routing, human review and provider data rules / AI lead |
| Operations | Privacy-safe logs, alerts, incident owner, quotas, costs and support process / operator |
| Commerce | Correct payment lifecycle, entitlements, failure/refund/cancellation tests and published terms / commercial owner |
| Accessibility | Mobile, keyboard, contrast, language, motion reduction and download checks / design |

Do not call the prototype an enterprise virtual data room or certified secure product. Notion is the current instance backend choice, not an assumed multi-tenant security boundary. Filtered views do not authorize access. Provider credentials remain server-side; browser hiding is not permission enforcement.

## MAIM learning sequence
Use fictional ventures and minimal personal information. Session 1: name the dependency and map roles. Session 2: distinguish statement/evidence/agreement. Session 3: scope a deliverable and classify feedback. Session 4: agree contribution rules and simulate change/dispute/exit. Session 5: make a go/revise/stop decision and explain it. Assess demonstrated reasoning, not upload volume or AI fluency. Keep minors out of real compensation workflows; establish appropriate consent before collecting learner data.
AMA uses these patterns for accountable delivery and deal qualification. MAIM teaches the mindset: make assumptions visible, preserve evidence, agree responsibilities and review decisions.

## Slicing Pie source boundary
Reviewed source: Mike Moyer, Slicing Pie Handbook, uploaded FREE SAMPLE; printed pp. 12–15 and 33. It describes at-risk unpaid contributions, adjusted tracking units and a freeze concept. Tracking units are not issued shares. No handbook is redistributed here; no affiliation, certification or complete method implementation is claimed. Detailed policies remain unreviewed unless supplied and explicitly adopted.

## Architecture decision proposed
Preserve the canonical platform and Stage A boundary. Add delivery, collaboration and learning as proposed experience profiles, not implemented modules. Reference the existing maim-client-workspace-builder skill for brand/configuration; the new delivery-control skill adds acceptance/change workflows.
Candidate records: Workspace(id, profile, tenant); Membership(workspace, projects, role, verified_identity); Source(version, provenance, visibility); Claim(source_location, review_state); Deliverable(baseline, functional_criteria, design_criteria); Change(before, after, approval); Contribution(policy_version, evidence, acknowledgment); Decision(actor, rationale, supersedes). Keep contribution scenarios separate from issued equity.
Record a contract decision for every shared record. Deny access before retrieval, export, download and AI processing. No frontend, integration, migration or deployment is authorized by this update. Existing integration table is directional: use one authoritative source per record; do not assume Airtable is required when the instance uses Notion.
Stage A exit remains acceptance of product spec, configuration/isolation and MVP scope. Add a synthetic cross-profile contract review before promoting code reuse.
