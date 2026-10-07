# Root Cause Analysis Template

Use this template after a major incident, or after a lower-priority incident that keeps coming back, to record what happened, why it happened, and what will stop it happening again.

## How to use this template

1. Copy this file and name the copy after the incident reference, for example `RCA-INC0012345.md`.
2. Replace the guidance in *italics* with your own content.
3. Start the document as soon as service is restored, while the details are fresh.
4. Look for causes in processes and systems, not in individuals. The aim is to fix the conditions that allowed the incident, not to assign blame.

---

## 1. Incident summary

| Field | Details |
| --- | --- |
| Incident reference | |
| Title | |
| Priority | |
| Service affected | |
| Detected (date and time) | |
| Resolved (date and time) | |
| Total duration | |
| Incident manager | |
| RCA author | |
| RCA date | |
| Status | Draft / In review / Final |

## 2. Impact

*Describe the impact in business terms, not technical terms.*

- **Who was affected:** *teams, locations or customers, with numbers where known*
- **What they could not do:**
- **Business impact:** *missed deadlines, lost transactions, manual workarounds, reputational impact*
- **Service level impact:** *any targets missed*

## 3. Timeline

*List the key events in order. Use one time zone throughout and say which one.*

| Time | Event | Source |
| --- | --- | --- |
| | *First sign of the problem* | *Monitoring alert, user report* |
| | *Incident logged* | |
| | *Major incident declared* | |
| | *Key diagnostic steps and decisions* | |
| | *Fix or workaround applied* | |
| | *Service confirmed restored* | |

## 4. Problem statement

*One or two sentences stating what failed, where, when and how widely. Describe the problem only. Do not include causes or solutions here.*

## 5. Analysis

### 5 Whys

*Start from the problem statement and keep asking "why?" until you reach something that can be changed to prevent a repeat. Five is a guide, not a rule. Support each answer with evidence.*

| # | Why? | Answer | Evidence |
| --- | --- | --- | --- |
| 1 | Why did the problem happen? | | |
| 2 | Why did that happen? | | |
| 3 | Why did that happen? | | |
| 4 | Why did that happen? | | |
| 5 | Why did that happen? | | |

### Contributing factors

*Things that did not cause the incident on their own but made it more likely, harder to detect or slower to fix.*

| Area | Contributing factor |
| --- | --- |
| People | *Knowledge, training, handover, availability* |
| Process | *Change control, testing, escalation, documentation* |
| Technology | *Monitoring gaps, capacity, configuration, resilience* |
| Supplier or environment | *Third-party services, dependencies* |

## 6. Root cause

*State the root cause in one or two sentences. A good root cause statement names something specific that can be fixed. "Human error" is not a root cause. Ask why the error was possible and why it was not caught.*

## 7. Resolution

- **What restored service:**
- **Was this a workaround or a permanent fix?**
- **If a workaround, what is the plan and date for the permanent fix?**

## 8. Corrective and preventive actions

*Every action needs one named owner and a due date. Action types:*

- *Corrective: fixes the cause of this incident*
- *Preventive: stops similar incidents from happening*
- *Detective: helps find the problem sooner next time*

| # | Action | Type | Owner | Due date | Status |
| --- | --- | --- | --- | --- | --- |
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |

## 9. Lessons learned

**What went well**

-

**What could be improved**

-

## 10. Sign-off

| Role | Name | Date |
| --- | --- | --- |
| RCA author | | |
| Service owner | | |
| Problem manager | | |

---

## Worked example

This fictional example shows the level of detail to aim for in sections 4 to 8.

**Problem statement:** Between 09:05 and 10:40 on a Monday, around 120 users in the Finance department could not sign in to Microsoft 365 from office desktops.

| # | Why? | Answer | Evidence |
| --- | --- | --- | --- |
| 1 | Why could users not sign in? | Sign-ins were blocked by a Conditional Access policy. | Sign-in logs showing the failure reason |
| 2 | Why did the policy block them? | A new policy requiring compliant devices applied to all users instead of the pilot group. | Policy assignment settings |
| 3 | Why did it apply to all users? | The policy was switched from report-only to on without the assignment being reviewed. | Audit log entry for the change |
| 4 | Why was the assignment not reviewed? | The change was raised as a standard change, which does not need a peer review. | Change record |
| 5 | Why was it a standard change? | The standard change catalogue does not separate low-risk changes from changes to identity policies that affect every user. | Change catalogue |

**Root cause:** The change process allowed identity policy changes that affect every user to be made as standard changes, without peer review.

| # | Action | Type | Owner | Due date | Status |
| --- | --- | --- | --- | --- | --- |
| 1 | Reclassify Conditional Access changes as normal changes that need peer review | Corrective | Change manager | *date* | Open |
| 2 | Require a report-only period and a review of its results before any policy is switched on | Preventive | Identity team lead | *date* | Open |
| 3 | Add an alert for a sudden rise in blocked sign-ins | Detective | Monitoring team lead | *date* | Open |

---

## Related documents

- [Major Incident Process](MajorIncidentProcess.md)
- [Escalation Guide](EscalationGuide.md)
- [Communication Templates](CommunicationTemplates.md)
- [Post-Incident Review Template](PostIncidentReviewTemplate.md)
