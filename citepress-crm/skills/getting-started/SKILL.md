---
name: getting-started
description: Use when someone first uses CitePress CRM from Claude, asks what it can do, cannot sign in, has no account, or gets a refusal from a CitePress CRM tool (not_permitted, not_in_scope, feature_unavailable, read_only, rate_limited, AI app access turned off).
---

# Getting started with CitePress CRM

1. **What it can do.** Call `citepress_help` with no topic for the list, or `topic: "about"`. Offer three
   things to try that fit what the person said, for example: find a contact and draft a follow-up; add a
   new contact and start them on a sales sequence; search Lead Finder for businesses in a city.
2. **Not signed in.** Any data tool starts the sign-in. If they have no account, `citepress_help`
   `topic: "account"` says how to create a workspace or join their team's. Say it once, plainly.
3. **What this connection can do.** Call `get_account_status`: workspace, role, plan or trial, which
   features are included, and the AI app switches. Use it before explaining any refusal.
4. **Refusals.** Read the tool's `message` and pass it on in your own words, with the one next step it
   gives (who to ask, or where in the CRM). For `feature_unavailable` with a plan named, say which plan
   includes it and, if the message has a link, give it once. Do not repeat it, and do not bring plans up
   unless the person's request needed the feature. `citepress_help` `topic: "troubleshoot"` lists every
   refusal.
5. **After each task**, offer at most two of the result's `nextSteps` as a short question.

Never ask for passwords or API keys in the chat. Sending email, deleting and spending Lead Finder
credits need the person's explicit yes; only then call again with `confirm: true`.
