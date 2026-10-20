# Change Control Board Impact Assessment

- **Project:** Montani Style Distributed Order Management System (DOMS)
- **Change Request:** Curbside Geo-Arrival Tracking
- **Requested by:** VP of Retail Operations & Store Experience
- **Prepared by:** Sophia Shaw, Noah Witzleb, Kenley Elmore
- **Date:** October 20, 2026

---

## Recommendation: DEFER

We recommend the CCB **defer** this request to a Phase 2 release after the Dec 4 final deliverable. The feature is valuable, but adding it now would put the core BOPIS and inventory work at risk.

---

## What Is Being Requested

Add a "Curbside Geo-Arrival Tracking" feature to BOPIS:

- When a customer is within 0.5 miles of a store, background GPS on their phone alerts store associates.
- A 3-minute delivery countdown timer starts.
- The system logs how fast each associate responds, for employee KPIs.

---

## Impact

| Area | Impact | Why |
|---|---|---|
| **Scope** | High | Needs a customer-facing mobile app, which is not in our current scope. Also adds geofencing, alerts, a timer, and KPI reporting. |
| **Schedule** | High | About 34 to 45 extra story points. Our team can do about 21 to 23 per sprint, and Sprint 3 is already full. The Dec 4 date would be at risk. |
| **Budget** | Medium | Estimated $90,000 to $140,000 extra, on top of the $750,000 to $1 million budget. |
| **Risk** | High | Privacy and legal issues with background location tracking. Employee concerns about KPI tracking. A 3-minute timer may be unrealistic. |
| **Resources** | High | Needs mobile development skills the team has not planned for. |

---

## Options

| Option | Result |
|---|---|
| Approve | Not feasible. Too much work for Sprint 3. |
| Reject | Not recommended. The feature has real value. |
| **Defer** | **Recommended.** Protects core delivery and allows time for legal review and planning. |

---

## Before Phase 2 Starts

1. Core BOPIS and inventory features are tested and stable.
2. Legal reviews the customer location consent.
3. HR and Retail Operations agree on how KPIs will be used.
4. The business confirms whether 3 minutes is a firm requirement.
5. Funding is identified for the extra cost.

**Short-term option:** Add an "I'm here" button to the BOPIS order so customers can tell the store when they arrive. No GPS needed.

---

## CCB Decision (to be completed by the CCB)

- [ ] Approve
- [ ] Reject
- [ ] Defer
