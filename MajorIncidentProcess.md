# Major Incident Process

## Objective

Restore service as quickly as possible while maintaining clear stakeholder communication.

## When this process applies

Use this process for any incident rated **Sev 1** or **Sev 2** in the [Escalation Guide](EscalationGuide.md), or any incident that is likely to reach that level.

If in doubt, declare a major incident. It is easier to stand a response down than to recover the time lost by starting late.

## Roles

| Role | Responsibility |
| --- | --- |
| Incident manager | Leads the response, makes decisions and owns the incident from declaration to closure. Coordinates the work but does not carry out the fix |
| Technical lead | Directs the investigation and recommends the fix |
| Communications lead | Sends updates to users and stakeholders on schedule |
| Resolver teams | Investigate and fix within their own area |
| Scribe | Keeps the timeline of events, decisions and actions |
| Service owner | Represents the business and decides on trade-offs that affect users |

In a small team one person may hold more than one role, but the incident manager should not also be the person doing the technical investigation.

## Process overview

| Phase | Goal | Output |
| --- | --- | --- |
| 1. Detection | Recognise that something is wrong | A confirmed issue with known impact |
| 2. Assessment | Decide how serious it is | A severity level and an incident record |
| 3. Escalation | Get the right people working on it | Named owners and an active investigation |
| 4. Communication | Keep everyone informed | Regular updates and a recorded timeline |
| 5. Resolution | Restore and confirm service | A closed incident |
| 6. Review | Learn and prevent a repeat | Lessons learned and preventative actions |

Phases 3, 4 and 5 overlap. Communication starts as soon as the incident is declared and continues until it is closed.

---

## Phase 1 - Detection

**Goal:** recognise that something is wrong and understand who is affected.

- Identify the issue, whether it comes from a monitoring alert, a user report or a rise in similar tickets
- Establish the impact: what can users not do?
- Determine the affected users: how many, in which teams and locations
- Check for recent changes that could be related
- Link duplicate tickets to a single parent incident

**Output:** a confirmed issue with a first view of its impact.

## Phase 2 - Assessment

**Goal:** decide how serious the incident is and record it.

- Assign a severity level using the [Escalation Guide](EscalationGuide.md)
- Assess the business risk: deadlines, revenue, safety, reputation and regulatory obligations
- Create the incident record, with the start time, symptoms and impact
- Declare a major incident if the severity is Sev 1 or Sev 2
- Name the incident manager

**Output:** an incident record with a severity level, and a named incident manager.

## Phase 3 - Escalation

**Goal:** get the right people working on the problem quickly.

- Notify the technical teams that support the affected service
- Open a single channel for the response, such as a conference bridge or chat channel
- Assign owners for each line of investigation
- Begin the investigation, starting with what changed most recently
- Involve suppliers early if their service or product is part of the problem
- Escalate to management in line with the [Escalation Guide](EscalationGuide.md)

**Output:** named owners, an active investigation and one place where the response is coordinated.

## Phase 4 - Communication

**Goal:** keep users and stakeholders informed so that they can plan around the incident.

- Notify stakeholders as soon as the major incident is declared
- Provide regular updates on a fixed schedule, even when there is no news
- Say what is known, what is not yet known, and when the next update will be
- Share any workaround as soon as it is confirmed
- Record progress, decisions and actions in the incident record as they happen

Use the [Communication Templates](CommunicationTemplates.md) for each message.

| Severity | Typical update frequency |
| --- | --- |
| Sev 1 | Every 30 minutes |
| Sev 2 | Every 60 minutes |

These are typical frequencies. Adjust them to match your own service level agreements.

**Output:** stakeholders who know the current position, and a complete timeline.

## Phase 5 - Resolution

**Goal:** restore service and confirm that it is working for users.

- Agree the fix or workaround, including the risk and how to reverse it
- Follow the emergency change process. An incident does not remove the need for approval
- Implement the fix
- Validate service restoration with monitoring and with affected users
- Keep monitoring for a period before standing the response down
- Send the resolution notice
- Close the incident, recording the cause as far as it is known and the fix applied

**Output:** service restored and confirmed, and a closed incident.

## Phase 6 - Review

**Goal:** learn from the incident and reduce the chance of a repeat.

- Complete the [Root Cause Analysis](RootCauseAnalysisTemplate.md) to explain why the incident happened
- Conduct a retrospective using the [Post-Incident Review Template](PostIncidentReviewTemplate.md)
- Identify lessons learned
- Define preventative actions, each with one named owner and a due date
- Track the actions to completion

**Output:** a completed root cause analysis, a post-incident review and tracked actions.

---

## Principles

- **Restore service first.** Find the root cause afterwards. A workaround that gets users working again is a good outcome.
- **One person leads.** Everyone should know who the incident manager is.
- **Communicate on schedule.** Silence causes more concern than "no change since the last update".
- **Record as you go.** A timeline written during the incident is far more accurate than one rebuilt afterwards.
- **Stay calm and factual.** Avoid blame and speculation, in the response channel and in updates.

## Related documents

- [Escalation Guide](EscalationGuide.md)
- [Communication Templates](CommunicationTemplates.md)
- [Root Cause Analysis Template](RootCauseAnalysisTemplate.md)
- [Post-Incident Review Template](PostIncidentReviewTemplate.md)
