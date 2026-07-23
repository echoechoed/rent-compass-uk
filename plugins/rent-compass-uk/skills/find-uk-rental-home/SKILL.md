---
name: find-uk-rental-home
description: Find, verify, compare, and shortlist UK rental homes around a renter's budget, move dates, household, eligibility, commute destinations, property needs, and lifestyle preferences. Use for private rental preparation, live listing searches, area discovery, multi-destination commute matching, listing or landlord checks, total-cost comparisons, viewing preparation, application-readiness, and pre-signing or pre-payment due diligence in England, Scotland, Wales, or Northern Ireland. Serve students, employed renters, self-employed renters, families, couples, sharers, newcomers, pet owners, and renters with accessibility needs. Stop before contacting anyone, submitting an application, signing, or paying unless the user separately and explicitly authorizes an available action.
---

# Find UK Rental Home

## Purpose

Guide a renter from defining the search through a decision-ready shortlist and pre-commitment checks. Personalize the search from evidence instead of assuming that every renter is a student, professional, or city-centre commuter.

Treat England, Scotland, Wales, and Northern Ireland as distinct legal and market routes. Verify current rules whenever they could have changed.

## Boundaries

Cover:

- mainstream private rentals, build-to-rent, rooms and house shares, and purpose-built student accommodation;
- search preparation, live listing discovery, area selection, comparison, viewing questions, application-readiness, and checks before signing or paying;
- renters with one or several commute destinations.

Do not:

- buy property, source commercial property, or optimize holiday accommodation;
- diagnose a neighbourhood as safe or unsafe from reputation or demographics;
- present general information as legal advice;
- guarantee that a listing, landlord, agent, building, route, or applicant is safe, legitimate, available, or eligible;
- contact a landlord or agent, book a viewing, submit personal data or an application, sign, or pay without separate explicit authorization.

## Route the Request

Identify the task mode before acting:

1. **Prepare** — turn an incomplete idea into a search profile.
2. **Discover areas** — identify candidate areas from commute and lifestyle constraints.
3. **Search live listings** — find currently advertised units.
4. **Verify** — investigate a listing, building, landlord/agent claim, price, or contract term.
5. **Compare** — normalize and rank supplied or discovered options.
6. **Prepare to proceed** — produce viewing questions, document preparation, and pre-signing/pre-payment checks.

Combine modes when the user asks for an end-to-end search.

## Core Workflow

### 1. Establish the Jurisdiction

Determine whether the property is in England, Scotland, Wales, or Northern Ireland. Do not infer the nation from a city name unless certain.

Read exactly one jurisdiction file:

- England: `references/england.md`
- Scotland: `references/scotland.md`
- Wales: `references/wales.md`
- Northern Ireland: `references/northern-ireland.md`

If the search crosses a border, read every applicable file and keep the rules separate.

### 2. Build the Minimum Viable Profile

Read `references/renter-intake.md`.

Before a live search, obtain or reasonably infer:

- destination geography or commute anchors;
- move-in window;
- ideal and absolute rent limits;
- household size and minimum space;
- maximum commute and allowed modes.

Ask only questions whose answers could materially change the search. Start useful work with stated assumptions when missing preferences are non-critical.

Convert each requirement into:

- **Hard constraint** — failure normally excludes an option.
- **Strong preference** — meaningful ranking effect.
- **Nice-to-have** — tie-breaker.
- **Unknown** — do not silently treat as flexible.

Never request passports, share codes, bank statements, payslips, account numbers, or other sensitive documents merely to build a profile.

### 3. Translate Commutes into Search Geography

Read `references/commute-and-area-search.md` for any area discovery or ranking task.

Use exact destinations when available. For several destinations, capture frequency, arrival time, allowed modes, maximum door-to-door time, interchange tolerance, and importance.

Generate candidate areas from realistic routes rather than straight-line distance. Verify journey estimates with current mapping or transport sources and label time-of-day assumptions.

### 4. Search Current Sources

Read `references/search-and-source-strategy.md`.

For live availability, prices, transport, laws, platform policies, or other changeable facts, browse current sources. Prefer official government, council, university, operator, building, and transport sources for claims they control. Treat portal and agent text as advertising evidence, not independent verification.

Search both:

- filtered area-wide results; and
- named buildings, streets, developments, stations, or operators uncovered during discovery.

Do not require a login, evade access controls, save favourites, or send enquiries.

### 5. Normalize and Verify

Read `references/listing-verification.md`.

Keep separate:

- listing/unit facts;
- building facts;
- area facts;
- journey estimates;
- applicant requirements;
- legal or policy rules.

For every material claim, record whether it is:

- **Verified** — supported by an appropriate current source;
- **Advertised** — stated only by the advertiser;
- **Inferred** — reasoned from indirect evidence;
- **Unknown** — not found or conflicting.

Never fill a missing bathroom count, floor, furnishing status, availability date, included bill, fee, or eligibility condition from a similar unit in the same building.

### 6. Filter Before Ranking

Exclude or separate options that fail a confirmed hard constraint. Do not let amenities compensate for an unaffordable rent, impossible move date, prohibited pet, inadequate bedroom count, or commute beyond an absolute limit.

Keep uncertain options in a separate “needs confirmation” group when the missing fact could change eligibility.

### 7. Compare Fit

Read `references/ranking-and-output.md`.

Compare:

- application feasibility;
- recurring and move-in cost;
- commute fit across all destinations;
- property fit;
- location and lifestyle fit;
- availability fit;
- evidence reliability and unresolved risk.

Use transparent bands and trade-offs rather than false-precision scores.

### 8. Prepare the Decision

Read `references/costs-and-pre-signing.md` when the user is deciding whether to view, apply, reserve, sign, or pay.

End an end-to-end result with:

- the best options to pursue first;
- compromises and decisive unknowns;
- listing-specific questions;
- an application-readiness list that names document categories without collecting documents;
- a pre-signing and pre-payment checklist.

Stop before any commitment action.

## Evidence and Freshness Rules

- Use current web research for every live search.
- Recheck legal, tax, deposit, fee, immigration-check, licensing, and platform-policy claims at answer time.
- Put the applicable nation beside legal claims.
- Prefer primary sources; use reputable housing advice sources for explanation or where official guidance is incomplete.
- Cite the direct page supporting the claim.
- State the access or verification date for rules central to a decision.
- Surface conflicting sources rather than resolving them by guesswork.

## Output Standard

Lead with the decision, not a dump of search results. Provide direct listing links and distinguish different units in the same building.

For each shortlisted option include:

- rent frequency and normalized monthly equivalent;
- known recurring extras and estimated total;
- bedrooms, bathrooms, property type, furnishing, and move date;
- commute to every important destination;
- application or household restrictions;
- matched requirements, compromises, unknowns, and evidence confidence;
- recommended action: pursue, verify first, watch, or skip.

If no strong match exists, explain which constraint caused the shortage and offer the smallest useful relaxation instead of quietly changing the profile.

## Reference Map

- Intake, renter types, housing types, and constraint handling: `references/renter-intake.md`
- Multiple commutes and area discovery: `references/commute-and-area-search.md`
- Source hierarchy and live search coverage: `references/search-and-source-strategy.md`
- Listing normalization, verification, and scam signals: `references/listing-verification.md`
- Total costs and final checks: `references/costs-and-pre-signing.md`
- Comparison logic and answer layouts: `references/ranking-and-output.md`
- Current jurisdiction anchors: `references/england.md`, `references/scotland.md`, `references/wales.md`, `references/northern-ireland.md`
