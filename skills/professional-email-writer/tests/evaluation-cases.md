# Evaluation cases for Professional Email Writer

These are **manual test prompts**, not evidence that Claude has already been tested. Test the installed skill with representative prompts and check both the content and the tone. Revise the skill when a consistent failure appears.

## Evaluation rubric (score each 0, 1, or 2)

1. **Intent/response** — answers the actual question or makes the necessary ask.
2. **Facts** — no invented statuses, fixes, approvals, root causes, access, deadlines, or business impacts.
3. **Format** — table only when helpful; preserves existing reply subject; appropriate length.
4. **Human tone** — direct, colleague-to-colleague, minimal boilerplate.
5. **Closing** — natural final sentence connected to the purpose, plus sign-off.

Target **9/10 or higher** for each scenario; any invented critical fact is an automatic failure irrespective of score.

## Case 1 — Manager portfolio update

**Prompt:** "Write my manager an update. SAGE launched Oct 19 and we're now working on adoption. Picker Accuracy training materials are still in progress. NOVA's next milestone isn't confirmed. Keep it short."

**Pass:** Compact table; accurate SAGE milestone; does not invent NOVA status; ends naturally after the table. **Fail:** Generic claims such as "measurable operational value" or fabricated NOVA delivery date.

## Case 2 — Single-project update

**Prompt:** "Tell my manager I finished the Supervisor Details page and will review it with operations next week."

**Pass:** Short prose, no four-column table; distinguishes finished work from planned review. **Fail:** Announces the entire dashboard is live.

## Case 3 — Question with known answer

**Prompt:** "Reply to: 'Where is the Staffing dashboard?' It is in the Power BI Supply Chain app under Operations > Staffing."

**Pass:** Answers in first sentence, retains `Re:`, ends helpfully. **Fail:** Only acknowledges the email or asks for information already known.

## Case 4 — Question with unknown cause

**Prompt:** "Reply to the director asking why Power BI totals don't match Cognos. We haven't investigated."

**Pass:** Says cause is not confirmed and what will be checked; no unverified claim that refresh timing is the cause. **Fail:** States a diagnosis as fact.

## Case 5 — Report issue; no diagnosis

**Prompt:** "A user wrote that the TML dashboard's Week 40 total looks wrong. The report name and week are already in the email. Respond; I haven't looked yet."

**Pass:** Refers to TML/Week 40; may ask for example values or screenshot, not report name/week; promises to look, not fix. **Fail:** Claims correction or asks again which report is affected.

## Case 6 — Verified resolution

**Prompt:** "Reply to the user. We refreshed the model, checked Week 40 against the source, and confirmed the totals now match."

**Pass:** States only those verified actions and optionally asks user to check. **Fail:** Invents root cause or says all historical totals have been validated.

## Case 7 — Oracle versus Snowflake mismatch

**Prompt:** "Email IT: Oracle is source of truth. Order 123 is 58 in Oracle and 52 in Snowflake; order 124 is 19 and 16. This affects Stocking report. Keep it natural."

**Pass:** Short email; `Details | Oracle | Snowflake` comparison; asks IT to investigate; names confirmed impact; avoids incident management jargon. **Fail:** Claims ETL failure as root cause.

## Case 8 — Follow-up on the mismatch

**Prompt:** "Follow up on that Oracle-Snowflake email. It's been two days and no one replied."

**Pass:** References earlier issue and asks for status without blame. **Fail:** Exaggerates severity or threatens escalation.

## Case 9 — AI agent pilot

**Prompt:** "Announce our supervisor AI agent pilot. Only five supervisors have access. It answers questions about new-hire utilization. Share the trial link as [Link]."

**Pass:** Clearly labeled pilot and limited audience; realistic example question; concrete starting action. **Fail:** Says available to all supervisors or promises correct answers.

## Case 10 — Automation launch

**Prompt:** "Announce a new automatic confirmation email after a user submits a valid analytics request through SAGE. Don't mention approvals."

**Pass:** Explains trigger, recipient experience, and whether action is needed, without inventing an approval. **Fail:** Claims manager review/approval is required.

## Case 11 — Simple follow-up

**Prompt:** "Follow up with IT about access to a table. I requested it Monday. Friendly, not too formal."

**Pass:** Two short paragraphs; specific ask; no 'gentle reminder' or invented deadlines. **Fail:** Excessively formal or passive-aggressive.

## Case 12 — Local rewrite only

**Prompt:** "Change only the last line of this email so it sounds natural: 'My focus remains on advancing these initiatives while ensuring they deliver measurable operational value.'"

**Pass:** Returns only a suitable closing sentence, not a rewritten whole email. **Fail:** Leaves the corporate jargon or invents a project commitment.

## Case 13 — Operational investigation with a remaining inventory gap

**Prompt:** "Rewrite my email to inventory control. The verified case pack setup was 12, corrected to 24. Receipt records show 744 eaches recorded and 1,488 expected based on actual cases. Shipment records show 744 recorded and 1,032 supported by picking detail. That leaves 456 expected, but system on-hand is 433. Ask them to recount location [Location]. Don't call the entire issue resolved."

**Pass:** Leads with the reviewed finding; short reconciliation table; calculates remaining 456 and gap 23 correctly; distinguishes supported/expected from physical count; asks for recount; natural closing. **Fail:** Calls 433 a physical count, says all inventory is reconciled, or implies the remaining 23 were shipped without evidence.

## Case 14 — Detailed evidence but short email

**Prompt:** "I've reviewed 37 store shipment rows for a case-pack issue. Twenty-one stores had loose-each picks and 16 had full cases. Rewrite my email for a warehouse supervisor: summarize the pattern, include the key discrepancy, and ask for a physical check. The transaction spreadsheet is available as an attachment."

**Pass:** Summarizes the store pattern without dumping 37 rows; refers to the actual provided attachment; directs a practical check. **Fail:** Invents store IDs or changes the totals, or rewrites into an overly formal report.

## Case 15 — Evidence is incomplete

**Prompt:** "Tell the team a SKU is short by 18 eaches, but I have only compared expected on-hand against system on-hand. No physical recount has occurred, and we don't know the root cause."

**Pass:** Labels 18 as the difference between calculated and system quantities, not confirmed physical shortage; states the cause is unknown; asks for a count. **Fail:** Claims 18 units are missing physically, accuses receiving, or says inventory is corrected.

## Test protocol

- Run at least three distinct cases, preferably all 15, in the target Claude setup.
- Test ambiguous prompts and whether the right reference is loaded when available.
- Compare outputs with preferred emails previously approved by the user.
- Record failing cases, the exact wording that failed, and the instruction you changed.
- Do not claim cross-model evaluation (Haiku/Sonnet/Opus) unless it has actually been performed.
