# Replying to questions and reported issues

Read the sender's original message when available. The reply should address *what they actually asked*, not a generic support script. Keep the existing `Re:` subject in email threads.

## Choose the right response

| Situation | Write this |
|---|---|
| **Known answer** | Direct answer first; one short explanation if needed; natural close |
| **Answer not verified** | Say what hasn't been confirmed and what will be checked; never invent a cause |
| **Power BI problem reported, not investigated** | Acknowledge the specific issue; ask only for essential missing detail; say you'll review it |
| **Investigation underway** | State what is being reviewed and whether recipient needs to do anything |
| **Cause confirmed** | Explain the verified cause and next step without blame |
| **Fix confirmed** | Say exactly what was corrected/validated; invite a targeted check if useful |
| **Expected behavior, not a defect** | Explain the definition/filter/refresh behavior neutrally and clearly |
| **Multi-person thread with partial answers** | Acknowledge the established update once; address the remaining question from the sender's role, without taking credit or inventing a commitment |

## Core rules

- If they asked "why?", **answer why** only when you know; otherwise say it's being checked.
- If they supplied report name, screenshots, examples, dates, and filters, **do not ask for them again**.
- Ask one or two targeted questions only when they're necessary to investigate. A screenshot is optional, not an automatic demand.
- The recipient shouldn't have to decode DAX, Snowflake, semantic models, or refresh architecture unless technical detail is helpful and warranted.
- When reporting a Power BI vs Cognos difference, don't assume a refresh timing issue; mention it only as a *possible* explanation if supported by context.
- Don't apologize for a confirmed issue unless warranted; don't declare a report "fixed" based on an assumption.
- A natural last sentence can be the next action itself: "I'll take a look and follow up with what I find."

## Multi-person threads, handoffs, and queue questions

Before writing a reply to a thread with several participants:

1. **Reconstruct the exchange:** Identify who raised each question, who answered it, what was confirmed, and what remains unanswered. Reply to the latest unresolved issue, using earlier messages as context.
2. **Respect ownership:** Attribute a status, decision, or ETA to the person or team who actually provided it. Do not repeat their answer as if it were the author's update, assign a new owner, or commit another team to work.
3. **Separate operational and system states:** A request being accepted into a sprint or planned for a date does *not* establish its status in SAGE, its workflow assignment or routing, who has access to view it, or whether a particular queue exists. Treat each as a separate fact requiring verification.
4. **Address the open question:** If someone asks how they can access, monitor, or manage a request queue, explain the confirmed path if supplied. Otherwise say access/routing needs to be checked, with a concrete next step that the author can reasonably take. Do not invent a link, role, permission, feature, or resolution.
5. **Keep the reply short and collegial:** A brief acknowledgment of adoption or collaboration may be appropriate, but avoid generic praise, repetitive summaries, policy lectures, and implying the recipient misunderstood the system.

**Example pattern (SAGE thread):** A team member confirms two requests are on an active sprint with a Tuesday estimate, then asks how they and a colleague can view their SAGE queue. The reply should not ask for another delivery update or claim queue access already exists. It should address visibility/routing as the remaining question; if those details are unverified, offer to check them or coordinate with the responsible owner. Avoid claiming the requests were submitted to or are already visible in SAGE unless the thread explicitly confirms that.

## Example: newly reported Power BI problem

**Subject:** Re: [Original Subject]

Hi [Name],

Thanks for bringing this to my attention.

Could you share which report or metric is affected and what you're seeing? A screenshot would also help if you have one.

I'll take a look and follow up once I've reviewed it.

Thanks,  
[Your Name]

*If the original email already identifies the report, remove that question and respond to its specifics.*

## Example: answer is available

**Subject:** Re: [Original Subject]

Hi [Name],

You can find [Report Name] in [confirmed location/link]. The [specific page] shows [confirmed information].

Let me know if you're having trouble accessing it.

Thanks,  
[Your Name]

## Example: cause still unknown

**Subject:** Re: [Original Subject]

Hi [Name],

I can see the difference you're referring to, but I haven't confirmed what's causing it yet. I'll review [known area to check] and follow up with what I find.

Thanks,  
[Your Name]

Use "I can see the difference" **only** if the sender's comparison or the author's review actually establishes that; otherwise write "Thanks for flagging the difference." These examples are patterns, not standard text to paste into every reply.
