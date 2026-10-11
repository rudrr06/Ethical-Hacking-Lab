# Google Dorking for Public Document Discovery

## Objective
Use Google search operators to find PDF files indexed under a specific domain, and understand the difference between discoverability and a confirmed security issue.

## Concepts
- `site:` limits results to a domain or site.
- `filetype:` filters results by file extension.
- Search results reveal what a search engine has indexed; they do not prove that a file is confidential, vulnerable, or improperly published.

## Lab environment and scope
- Tool: web browser and Google Search.
- Query recorded in the screenshot: `site:skills-factory.com filetype:pdf`.
- Scope: public search results only. No authentication bypass or access-control testing is shown.

## Procedure
1. Open Google Search in a browser.
2. Enter `site:skills-factory.com filetype:pdf` and submit the query.
3. Review the result titles, snippets, and displayed domain to confirm that the results are associated with the intended domain.
4. Open only material that appears intended for public access and that you are permitted to review.
5. Record the query and high-level result types. Do not download or republish personal, confidential, or copyrighted material.
6. If a potentially exposed sensitive file is found during an authorised assessment, report its URL privately to the site owner instead of sharing its contents.

## Observed result
The screenshot shows multiple PDF results associated with the queried domain, including course/brochure-style documents. This supports that the operators returned indexed PDFs; it does not establish that any result was sensitive.

## Evidence
![Google Search results for the recorded query](evidence/google-dorking.png)

## Interpretation and limitations
Search-engine indexing is a discovery technique, not a vulnerability verdict. Confirm intended audience, data sensitivity, and access policy before reporting exposure. Results can change over time and may be incomplete.

## Defensive recommendations
Review public web directories before publication, remove unintended sensitive files, use appropriate access controls, and request search-engine removal when a sensitive resource has already been indexed.

## Reference
[Google Search operators](https://support.google.com/websearch/answer/2466433)
