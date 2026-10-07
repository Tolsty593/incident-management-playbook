# Post-Incident Review Template

A post-incident review is a short, structured meeting held after a major incident. Its purpose is to learn from how the incident was handled and to agree improvements.

It works alongside the [Root Cause Analysis](RootCauseAnalysisTemplate.md):

- The **root cause analysis** explains *why the incident happened*.
- The **post-incident review** looks at *how well we detected it, responded to it and communicated about it*.

## Ground rules

- **Blameless.** Assume everyone acted with good intentions and the information they had at the time. Discuss decisions and systems, not individuals.
- **Facts first.** Agree the timeline before discussing opinions.
- **Everyone contributes.** The person closest to the problem often has the most useful insight.
- **Leave with actions.** Every improvement needs one named owner and a due date.

## When to hold the review

Hold the review within a few working days of the incident being resolved, while details are fresh. Invite the incident manager, the engineers who worked on the incident, the service owner, and a representative of the affected users where possible.

## Suggested agenda (45 minutes)

| Time | Item |
| --- | --- |
| 5 min | Purpose and ground rules |
| 10 min | Walk through the timeline |
| 15 min | What went well and what could be better, phase by phase |
| 10 min | Agree actions, owners and dates |
| 5 min | Summary and next steps |

---

## 1. Review details

| Field | Details |
| --- | --- |
| Incident reference | |
| Incident title | |
| Priority | |
| Date of incident | |
| Date of review | |
| Facilitator | |
| Attendees | |
| Link to root cause analysis | |

## 2. Incident summary

*Two or three sentences: what happened, who was affected, how long it lasted and how service was restored.*

## 3. Key measurements

*Record the actual times and compare them with your targets.*

| Measure | Actual | Target | Met? |
| --- | --- | --- | --- |
| Time to detect (start of impact to first alert or report) | | | |
| Time to acknowledge (first alert to an engineer starting work) | | | |
| Time to escalate (acknowledgement to major incident declared) | | | |
| Time to first communication (declaration to first update sent) | | | |
| Time to restore (start of impact to service restored) | | | |
| Number of updates sent, and whether they were on schedule | | | |

## 4. Review by phase

*The phases match the [Major Incident Process](MajorIncidentProcess.md).*

| Phase | What went well | What could be better |
| --- | --- | --- |
| Detection | | |
| Assessment | | |
| Escalation | | |
| Communication | | |
| Resolution | | |

### Questions to prompt discussion

**Detection**

- How did we find out? Was it monitoring or a user report?
- Could we have found out sooner?

**Assessment**

- Was the priority set correctly the first time?
- Did we understand the impact on users quickly enough?

**Escalation**

- Did we reach the right people quickly?
- Were contact details and on-call rotas correct?
- Did everyone know who was leading the incident?

**Communication**

- Were updates clear, regular and free of jargon?
- Did users and stakeholders know where to look for updates?
- Did anyone find out about the incident later than they should have?

**Resolution**

- Did we have the access, tools and documentation we needed?
- Was there a workaround we could have offered sooner?
- How did we confirm that service was fully restored?

**Overall**

- Where did we get lucky?
- What would have made this incident worse?
- If the same thing happened tomorrow, what would we do differently?

## 5. Lessons learned

*Summarise the main points from the discussion in plain language.*

1.
2.
3.

## 6. Actions

| # | Action | Owner | Due date | Status |
| --- | --- | --- | --- | --- |
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

## 7. Follow-up

| Field | Details |
| --- | --- |
| Date to review progress on actions | |
| Where this review is stored | |
| Who the review has been shared with | |
| Knowledge base articles or procedures to update | |

---

## Related documents

- [Major Incident Process](MajorIncidentProcess.md)
- [Escalation Guide](EscalationGuide.md)
- [Communication Templates](CommunicationTemplates.md)
- [Root Cause Analysis Template](RootCauseAnalysisTemplate.md)
