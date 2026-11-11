---
name: prospect-with-lead-finder
description: Use when someone wants new prospects - businesses of a kind in a place - from CitePress CRM's Lead Finder.
---

# Prospect with Lead Finder

1. `lead_finder_search` with what and where (for example category "bakery", city "Pune"). Searching is
   free; emails and phones are masked until unlocked.
2. Show the best results: name, place, which checks they passed. `lead_finder_business` for any one in
   full.
3. Before unlocking, `lead_finder_quote` for the businesses they picked and `lead_finder_credits` for the
   balance. Tell them the cost in credits. Unlocking spends credits: only with their yes, and with
   `confirm: true` and `maxCredits` set to the quote.
4. Add the unlocked ones to the CRM with `lead_finder_add_to_crm`, then offer to draft first emails.

If Lead Finder is off for the workspace, the tools say so and who can start it; pass that on.
