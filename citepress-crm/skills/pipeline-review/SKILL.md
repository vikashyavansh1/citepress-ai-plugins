---
name: pipeline-review
description: Use when someone asks for a pipeline or sales review in CitePress CRM - what is in each stage, what is stuck, what to do this week.
---

# Pipeline review

1. `list_leads` for every stage, or one stage if they named it. Report each open stage: count, value,
   and the leads that matter most by value.
2. For the leads they ask about, `get_lead` for notes, next step and history. Point out leads with no next
   step or no recent activity.
3. Propose at most five actions for the week, each one a tool call they can approve: a follow-up draft
   (`create_email_draft`), a stage change (`set_lead_stage`), a note (`add_lead_note`).
4. Make no change without their yes.

`list_leads` is in the full tool set. If it is refused with `feature_unavailable`, say what the message
says (the plan that includes it, and the link if one is given) once, then offer what the everyday tools
can still do: search contacts and draft follow-ups.
