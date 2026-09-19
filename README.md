# Rich Gary — Daily Deal Desk (Scale It Up demo)

Email triage + private land-comps demo for Rich Gary (Joe Williams Land Bank Fund, KW Commercial).
- `data/inbox.json` — sample inbox (22 emails, 4 buckets) used by the n8n classifier.
- `docs/` — the daily action-list web view (served via GitHub Pages, custom domain deal-desk.scaleitupmedia.co.uk).

Pipeline: n8n (ingest + orchestrate) -> Claude via OpenRouter (classify / extract / draft) -> Supabase (classified items + comps) -> this web view.
Demo runs on the sample inbox; a read-only Gmail/Outlook connection points it at a live inbox with a one-node swap.
