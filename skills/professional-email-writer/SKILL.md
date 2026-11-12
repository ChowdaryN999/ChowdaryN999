---
name: professional-email-writer
description: Write, reply to, and improve natural, concise professional business emails. Use for manager or executive project updates, Power BI or analytics questions, reported report issues, IT and data-discrepancy escalations, launch announcements for reports/AI agents/automations, meeting requests, follow-ups, and stakeholder communication. Adapt structure to the situation instead of using one email template.
---

# Professional Email Writer

Write emails a capable, approachable colleague would actually send. Be clear and direct, not stiff, generic, or overly polished. Preserve the sender's voice and the facts they provide.

## Decide before drafting

1. Identify the **situation**: new message, reply to a thread, update, answer, investigation, escalation, launch, or follow-up.
2. Identify the **recipient and purpose**: what they need to understand or do after reading.
3. Separate **confirmed facts** from unknowns, assumptions, and things still being investigated.
4. Choose the relevant playbook below. Read **only** the reference file(s) that match the request.
5. Draft a copy-ready email and make the ending sound natural for that situation.

## Select the playbook

| Situation | Read this reference | Default format |
|---|---|---|
| Updates covering several projects for a manager or executive | [references/project-updates.md](references/project-updates.md) | Short opener + status table + natural close |
| Responding to a user's question or someone reporting a Power BI/report issue | [references/email-replies.md](references/email-replies.md) | Short reply; answer or next step first |
| Oracle vs Snowflake discrepancies, technical problems that need IT help | [references/it-escalations.md](references/it-escalations.md) | Plain-language issue + evidence + specific ask |
| Announcing a Power BI tool, AI agent, workflow, or automation | [references/launch-announcements.md](references/launch-announcements.md) | What's new + usefulness + how to start |
| Requests, follow-ups, meeting invitations, recognition, disagreement, other business emails | [references/general-emails.md](references/general-emails.md) | Concise, purpose-led paragraphs |

If more than one applies, use the **primary purpose** and borrow only a necessary rule from a second reference. A reply to a question about a data discrepancy should **answer the question** if the answer is known; don't automatically write an escalation.

## Non-negotiable writing rules

- **Lead with the point.** No ceremonial introductions or unnecessary background.
- **Use ordinary language.** Favor "The numbers aren't matching" over "A data integrity inconsistency has been identified."
- **Be respectful and confident.** Sound like a colleague, not a policy document or customer-service bot.
- **Don't invent details.** No made-up project status, deliverables, root causes, deadlines, impacts, launches, links, fixes, owners, or actions already performed.
- **Use the information already provided.** Don't ask someone to repeat a report name, example, or screenshot that is already in the thread.
- **Don't overpromise.** State what you'll review or check, not that you fixed something or know the cause without evidence.
- **Choose structure deliberately.** Tables for several projects or useful side-by-side comparisons; short prose for ordinary replies. Bullets only when they make scanning easier.
- **Write a purposeful ending every time.** Close with the actual next step, a reasonable offer to discuss, or a direct request, then an appropriate sign-off. Do **not** automatically repeat a stock closing.
- **Match the original message.** When replying, keep the thread's subject and context. When rewriting, preserve the sender's meaning, specifics, and intended level of directness.
- **Be careful with internal data.** Include only the details needed by the recipients; don't add sensitive personal or business data just to make an example look realistic.

## Anti-AI language filter

Remove phrases that could appear in almost any corporate email, especially:

- "I hope this email finds you well"
- "I'm reaching out to..." when "We noticed..." or "Can you..." would work
- "measurable operational value," "high-impact opportunities," "addressing dependencies"
- "leverage," "synergies," "seamless," "game-changing," "unlock the power of AI"
- "At your earliest convenience," "Please be advised," "Thank you for your continued support"

Do not replace them with another kind of canned corporate phrasing. Prefer concrete facts and everyday verbs. Natural contractions are fine.

## How to handle incomplete information

- If enough context is available, **draft now** using only supported details.
- Use a small placeholder such as `[Report Name]`, `[Link]`, or `[Next Step]` only if essential to a usable draft.
- If a missing fact makes a truthful answer impossible, ask **one targeted question**, or draft a version that clearly says what is not yet confirmed.
- If users are reporting an issue, distinguish **reported**, **being checked**, **cause confirmed**, and **resolved**. Never silently upgrade a report into a diagnosis or a fix.

## Output and revisions

- By default, return **one finished email** with a subject for a new message. Preserve `Re:` for an existing thread. Include greeting, body, purposeful closing, and sign-off.
- Avoid prefacing the draft with writing theory. Give explanations or alternatives only if requested.
- If asked to revise a line, change that line rather than rewriting everything. If asked for the full email, deliver the full email incorporating the chosen revision.
- If requested, provide 2–3 **meaningfully different** tone options, not superficial synonym swaps.
- Use `[Your Name]` for an unknown sender; retain the supplied sender's name/signature when available.

## Silent final check

Before sending: Is the first sentence useful? Does it answer or ask for the right thing? Is every factual claim supported? Is the format right for the situation? Could a colleague plausibly have written this? Is the ending meaningful and non-repetitive? Remove anything that fails.

For manual evaluation prompts and pass/fail checks, see [tests/evaluation-cases.md](tests/evaluation-cases.md) **only when testing or reviewing the skill**.