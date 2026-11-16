# Operational investigations, inventory reconciliations, and findings emails

Use when the sender has **already analyzed an operational issue** and needs to explain what happened, show evidence, distinguish remaining uncertainty, and ask another team to act. Examples include wrong case packs, inventory variances, receiving/shipping discrepancies, warehouse location counts, transaction exceptions, and operational root-cause summaries.

This is **not** the same as a first report of a Power BI problem or a simple request for IT to investigate. Here the sender is communicating *findings from an investigation*. Write as an experienced operations or analytics colleague, not as a formal audit report.

## Lead with the decision-relevant result

Use this logic, in this order:

1. **Finding:** What was reviewed and what the evidence shows. Start with the practical conclusion, not the timeline of every lookup.
2. **Evidence:** Present the few facts or counts that support the finding, ideally a compact comparison or reconciliation table.
3. **Remaining gap:** Clearly separate unexplained differences, assumptions, potential consequences, and facts that still require validation.
4. **Action needed:** Ask the specific recipient to check, recount, correct, confirm, or decide something. End with a natural, proportionate closing.

Do not use four literal section headings in every short email. The four parts are a thinking framework, not a mandatory template.

## Truth and reconciliation rules

- Preserve source terminology and units: **cases**, **eaches**, **loose eaches**, **case pack**, **on-hand**, **pick**, **shipped**, **received**, **counted**. Don't treat one as equivalent to another.
- Label values as **system recorded**, **actual/physically verified**, **calculated/expected**, or **reported**. Never silently upgrade a calculation or inference into a physical count.
- Check the arithmetic of any reconciliation *using only the figures supplied*. If the numbers don't reconcile or the scope/time cutoff isn't clear, mark the difference as unresolved rather than inventing transactions.
- Compare like with like: same item, location, time period, unit of measure, and transaction scope. Include date/cutoff only when supplied or essential.
- Separate **confirmed root cause** from **possible contributing factor** and **remaining unexplained variance**. A corrected case pack does not automatically explain every remaining on-hand difference.
- Don't claim a store was overcharged/undercharged or received the wrong amount without evidence for billing and physical receipt. Prefer "the system recorded X, while the available pick/shipment evidence indicates Y" when appropriate.
- If no physical recount occurred, don't say the quantity was physically confirmed. If a case pack was changed, don't say inventory was reconciled unless it was actually reconciled.
- Don't imply "no open orders" or "no short shipments" unless that was actually checked.
- Don't invent location IDs, order counts, case quantities, corrections, owner assignments, approvals, or completed actions.
- If an operational issue might involve sensitive business or customer details, include the minimum necessary for the recipient; avoid putting large record-level extracts in the email unnecessarily.

## Evidence presentation

For a concise numerical comparison, use a table like:

| Measure | System Recorded | Calculated / Verified |
|---|---:|---:|
| Received | [recorded eaches] | [supported actual eaches] |
| Shipped | [recorded eaches] | [supported actual eaches] |
| Remaining on-hand | [system eaches] | [expected or counted eaches, clearly labeled] |

Only combine numbers in a single row when they are comparable; a counted snapshot and an expected balance are different measures and may warrant separate rows.

- If the investigation is mostly narrative, **do not force a table**.
- When there are dozens of rows (stores, orders, locations), summarize the pattern and reference a **provided** attachment or linked evidence. Do not claim an attachment exists unless supplied; otherwise offer to share the detail or use a placeholder such as `[Detailed transaction breakdown]`.
- Put the most important comparison in the body, not a screenshot dump. Use bullets for two or three key observations if useful.
- Preserve the subject of an existing thread; for a new email use a descriptive subject like `Item [ID] | Inventory Review and Location Check`.

## Natural closing

Ask directly for the action the recipient can actually take:

> Could you please have location [Location] rechecked to confirm the on-hand quantity?

If the next step depends on the result, state that condition:

> Once the count is confirmed, we can review whether an inventory adjustment is needed.

Don't prescribe a system update before the count is verified, unless the user explicitly confirms that the correction is authorized and appropriate. Avoid generic "operational excellence," "proactive mitigation," or "ensure data integrity" conclusions.

## Adaptable example (fictional values)

**Subject:** Re: Item [ID] | Inventory Difference

Hi [Name],

I reviewed the receiving and shipping activity for item [ID]. The case pack appears to have been entered as 12 instead of 24, which would affect the quantities recorded for full cases.

Here is the summary based on the records reviewed:

| Measure | Recorded | Calculated / Expected |
|---|---:|---:|
| Received (eaches) | 600 | 1,200 |
| Shipped (eaches) | 600 | 840 |
| Expected remaining (eaches) | — | 360 |
| Current system on-hand (eaches) | 342 | — |

That leaves an 18-each difference between the expected balance and the current on-hand quantity. I haven't confirmed what accounts for that difference.

Could you please have location [Location] rechecked? Once we have the count, we can determine whether any correction is needed.

Thanks,  
[Your Name]

**Note:** The example is only a writing demonstration. Don't reuse its numbers, assumptions, or root cause in a real investigation.

## Routing overlap

- **Explaining completed operational analysis to a supervisor, manager, inventory control, or operations team:** use this reference first.
- **Asking IT to investigate an unexplained source-system mismatch:** use `it-escalations.md` first.
- **Only acknowledging a newly reported issue:** use `email-replies.md` first.
- **Answering an actual user question:** answer it first and borrow only the evidence/reconciliation rules needed here.

## Quality check

Before sending, ask silently: Is the bottom line in the first paragraph? Are units and arithmetic consistent? Are recorded, calculated, and physically verified values distinguished? Is any remaining difference clearly identified as unresolved? Is the requested action specific and feasible? Is the email shorter than the raw investigation without leaving out material evidence?
