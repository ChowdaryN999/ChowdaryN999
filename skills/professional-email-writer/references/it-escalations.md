# Asking IT to investigate a data or system problem

Use a straightforward colleague-to-colleague tone. Describe what was noticed, show a concrete example, and ask the IT team to take a look. Don't turn an ordinary investigation request into a formal incident report.

## Ordinary Oracle vs Snowflake discrepancy

When Oracle is *confirmed* as the source of truth and a Snowflake result differs:

1. Say which table, metric, or group of records isn't matching.
2. Mention Oracle as the source of truth, but only if confirmed by the user.
3. If actual comparative values are provided, show a small `Details | Oracle | Snowflake` table. Otherwise use a placeholder table or plain prose, based on what the user asks.
4. Ask IT to review the difference and help explain it. **Do not diagnose** ETL logic, joins, latency, the warehouse, or Oracle without evidence.
5. Mention the affected report/process if known. End with a short request for an update.

## Approved example

**Subject:** Data Mismatch Between Oracle and Snowflake

Hi Team,

We noticed some differences between the data in Oracle and Snowflake for [Table Name].

Oracle is our source of truth, but the numbers in Snowflake aren't matching. I've included a few examples below for reference.

| Details | Oracle | Snowflake |
|---|---|---|
| [Record / Date] | [Value] | [Value] |
| [Record / Date] | [Value] | [Value] |

Could you please take a look and help us understand what's causing the mismatch?

This is affecting [Report / Process], so we'd appreciate an update once you've had a chance to investigate.

Thanks,  
[Your Name]

## Adjust to the stage

- **Initial issue:** Short statement, evidence, question. No presumed diagnosis.
- **Follow-up:** Reference earlier message/ticket when provided; "Have you had a chance to look into this?" is often enough.
- **Identified cause:** Explain only the confirmed finding, impact, and next action.
- **Correction verified:** State what changed and how it was checked, if provided. Ask for confirmation only if useful.
- **Urgent or business-critical impact:** Include the actual operational consequence and requested timing if supplied; use an established incident route if the user provides one. Direct and calm can still be urgent.

## Keep analysis separate from the email

Before escalating, it may be useful to compare the same business dates, grain, filters, time zone, and refresh cutoff. These are optional investigation checks, **not claims to insert into an email** and not a reason to delay a requested draft.

Avoid phrases such as "data integrity escalation," "downstream analytics platform," "determine the scope and root cause," "expected remediation/backfill," and "measurable operational impact" unless the user's situation specifically calls for that language.

Don't assign blame to Oracle, Snowflake, data engineering, or a named owner based solely on the mismatch.
