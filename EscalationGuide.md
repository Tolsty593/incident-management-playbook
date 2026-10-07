# Escalation Guide

This guide defines the severity levels used across the playbook and explains when and how to escalate.

## Severity Levels

| Level | Definition | Typical examples | Response |
| --- | --- | --- | --- |
| **Sev 1** | Critical outage affecting all users | Email or sign-in down for the whole organisation; a business-critical system unavailable; a security incident in progress | Immediate. Follow the [Major Incident Process](MajorIncidentProcess.md) |
| **Sev 2** | Significant degradation affecting multiple users | A site or department cannot work; a key system is very slow or partly unavailable | Urgent. Follow the [Major Incident Process](MajorIncidentProcess.md) |
| **Sev 3** | Limited impact with workaround available | One user or a small group affected; a feature is not working but work can continue | Handled in the normal queue, by priority |
| **Sev 4** | Minor issue or service request | A cosmetic fault; a how-to question; a request for access or software | Handled in the normal queue |

### Setting the severity

Severity depends on impact and urgency, not on who reports the problem.

- **Impact:** how many people are affected, and how badly?
- **Urgency:** how quickly does the business need it fixed? Is there a deadline, or a risk to safety, revenue or reputation?

Raise the severity if the impact grows, a workaround stops working or a deadline approaches. Lower it when a workaround is in place and users can carry on.

### Severity and priority

Where a ticketing system uses priority names, they map to severity like this:

| Severity | Priority |
| --- | --- |
| Sev 1 | Critical |
| Sev 2 | High |
| Sev 3 | Medium |
| Sev 4 | Low |

## Types of Escalation

- **Functional escalation** passes the incident to a team with more specialist knowledge or access, for example from the service desk to the network team.
- **Hierarchical escalation** informs or involves management, to get decisions, resources or wider communication.

A serious incident usually needs both.

## Escalation Matrix

| Level | Who | Escalate to this level when |
| --- | --- | --- |
| Level 1 | Service desk | First contact. Log, assess and resolve where possible |
| Level 2 | Technical support teams | Level 1 cannot resolve the issue with its access or knowledge, or the time allowed at Level 1 has passed |
| Level 3 | Specialist engineers and suppliers | The problem needs a change to a system, a supplier's involvement or specialist knowledge |
| Management | Service delivery manager and service owner | Any Sev 1 or Sev 2 incident, a missed target, a dispute over ownership, or a decision that affects the business |

## When to Escalate

Escalate when any of these is true:

- The incident is Sev 1 or Sev 2
- The problem is outside your access, knowledge or authority
- The time allowed at your level has passed without progress
- The impact is growing
- More than one team is needed and no one is coordinating
- A supplier is not responding within their agreed time
- You are not sure. Escalating early costs little, and escalating late costs a lot

## What to Include

A good escalation lets the next team start work without going back to the user.

- [ ] Incident reference and severity
- [ ] One-sentence summary of the problem
- [ ] Who is affected, and the business impact
- [ ] When it started and what changed
- [ ] Exact error messages, screenshots and logs
- [ ] Everything already tried, with results
- [ ] Any workaround in place
- [ ] Who to contact, and how

## Escalation Principles

- **Escalate early.** Do not wait until a target has been missed.
- **Communicate clearly.** State the problem, the impact and what you need from the person you are escalating to.
- **Track ownership.** At every moment one named person owns the incident. Handing over the work does not hand over the ownership until the next person confirms that they have it.
- **Maintain regular updates.** Keep the user and stakeholders informed while the incident moves between teams.

## Related documents

- [Major Incident Process](MajorIncidentProcess.md)
- [Communication Templates](CommunicationTemplates.md)
- [Root Cause Analysis Template](RootCauseAnalysisTemplate.md)
- [Post-Incident Review Template](PostIncidentReviewTemplate.md)
