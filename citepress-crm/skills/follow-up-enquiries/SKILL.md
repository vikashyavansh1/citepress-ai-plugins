---
name: follow-up-enquiries
description: Use when someone wants to follow up with new enquiries, recent contacts, or a named person in CitePress CRM by email or a sales sequence.
---

# Follow up enquiries

1. Find the people: `search` with a name, email or company, or `list_contacts` with `search`. If there
   are several matches, show them (name, email, company) and ask which.
2. Read before writing: `fetch` (or `get_contact`) for their leads and recent activity, so the email
   refers to what actually happened.
3. Draft, do not send: `create_email_draft` with `contactId`, a subject and the text. Show the person the
   draft and the link to it in the CRM.
4. Offer the choices from `nextSteps`: send it now (needs their yes, then `send_email_draft` with
   `confirm: true`), schedule it, or start them on a sales sequence (`list_sales_sequences`, then
   `enroll_in_sales_sequence`).
5. For several people, draft one at a time and summarise at the end: who got a draft, who was skipped
   and why.

If a tool is refused, follow the getting-started skill's step 4.
