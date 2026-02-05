# Search expectations and result template

When you perform web searches for project reports, present results in a consistent, verifiable format so other team members can review, follow up and archive sources.

Required fields for every article (use this template):

- **Title:** Full article title as published
- **URL:** Clickable link (copy the canonical link)
- **Publisher / source:** e.g., Hong Kong Fire Services Department, RTHK, HK01, SCMP
- **Date published:** YYYY-MM-DD (or best approximation)
- **Date searched:** YYYY-MM-DD (when you ran the query)
- **Summary (2–3 lines):** Key facts, what the article says about the incident
- **Relevance to project goals:** Why this is useful for the team (timeline, official statements, technical detail, public reaction, policy change, etc.)
- **Follow-up suggestions:** What the team should do next (e.g., extract timeline, contact spokesperson, archive paywalled article, check official press release)
- **Credibility / paywall note:** Is the article behind a paywall? Is it an official source or opinion piece? Any reason to treat it cautiously.

Optional but recommended fields:

- **Search query used:** The exact query string you ran (helps reproducibility)
- **Screenshot / archived link:** Wayback URL or a screenshot file path if content may change or is paywalled

Formatting and style

- Include 5–8 articles per incident search: a mix of official sources (FSD, gov), public broadcaster (RTHK), and independent press (HK01, SCMP, The Standard).
- Order results by priority: official statements first, then major outlets, then local opinion/analysis.
- Keep item summaries factual and cite the sentence or paragraph that justifies your summary.

Suggested search queries (tailor for the incident):

- "Tai Po fire Nov 2025"
- "Tai Po flat fire 2025 Fire Services Department press release"
- "Tai Po building fire investigation 2025 cause"
- "Tai Po fire casualties response time 2025"

Quick commands to run locally (copy/paste) for basic checks:

```
curl -sS "https://www.hkfsd.gov.hk" | grep -i "Tai Po" -n || true
curl -sS "https://www.rthk.hk" | grep -i "Tai Po" -n || true
```

Archiving and paywalls

- If an article is paywalled (e.g., SCMP), note that in the "Credibility / paywall note" and either capture a screenshot or an archived copy (Wayback) and save it to the group folder.

Deliverable format

- Save results in the group's `reportMediaCoverage.md` or `WebSearchReport.md` using the template above.
- Add your short running notes to `process.log` (what you searched, sites checked, any network issues) so ProjectMetaDirector can track progress.

End of expectations.
