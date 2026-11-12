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

## Core rules

- If they asked "why?", **answer why** only when you know; otherwise say it's being checked.
- If they supplied report name, screenshots, examples, dates, and filters, **do not ask for them again**.
- Ask one or two targeted questions only when they're necessary to investigate. A screenshot is optional, not an automatic demand.
- The recipient shouldn't have to decode DAX, Snowflake, semantic models, or refresh architecture unless technical detail is helpful and warranted.
- When reporting a Power BI vs Cognos difference, don't assume a refresh timing issue; mention it only as a *possible* explanation if supported by context.
- Don't apologize for a confirmed issue unless warranted; don't declare a report "fixed" based on an assumption.
- A natural last sentence can be the next action itself: "I'll take a look and follow up with what I find."

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
