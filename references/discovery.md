# Source collection and relevance

## Supplied links and browser history

Use only the requested source and relevant browser profile. Open the history/device surface or use a supported focused history API when authorized. For synced device tabs, record the device name and each observed link; do not assume all device entries are exposed to automation.

Enumerate with visible scrolling or pagination and maintain a coverage checkpoint (count, last visible title/link and whether the end was observed). If the tool exposes only part of a list, try its documented scrolling/navigation method. If the remainder still cannot be read, record `coverage_incomplete` and the exact continuation point. Ask for user scrolling only if necessary; continue processing accessible entries meanwhile.

Strip tracking parameters where safe, but retain job/requisition identifiers. Repeated source URLs, company career pages and recruiters' reposts may all refer to one job; keep their source provenance under one application record. If a link is a general directory, find the specific relevant opening before applying. Do not treat every browser-history page as an application request.

## LinkedIn discovery in signed-in Chrome

Use the Chrome profile belonging to the candidate. Prefer LinkedIn Jobs search and relevant hiring posts over indiscriminate feed scrolling. Inspect the resume first to select role families, search terms and transferable skills. Apply the user's preferences for location, remote/onsite, seniority, domain and sponsorship. Use targeted searches and visible filters; inspect the actual posting before deciding fit.

When requested, scroll the candidate's feed or hiring posts to discover openings. Read referenced original posts when needed for the employer, role or contact address. Use LinkedIn as a discovery source and follow the actual employer's application link when available. Use Easy Apply if appropriate and authorized; verify the selected resume and any remembered form answers before submission.

Make search bounded and resumable. If no quantity or time limit is supplied, select a modest initial batch (for example 10–20 strong matches), state that assumption, and process it before expanding within the requested scope. Record the query/filter, last reviewed page or posting, and date. Stop on a clear user limit, exhausted relevant results, access restrictions, or a sustained run of poor matches; summarize how to continue. Never promise unattended future discovery without an explicitly configured automation.

## Fit decision

Record a short explanation using evidence, not just a keyword score:

- Required skills met through actual projects or employment; distinguish hands-on use from related knowledge.
- Experience and level: compare dates and responsibility, allow sensible adjacent levels, and flag hard minimums that are not met.
- Domain: distinguish a preference for product/startup experience from a mandatory regulated-domain qualification.
- Location and eligibility: use confirmed work authorization for the job country. Willingness to relocate does not imply visa eligibility or sponsorship availability.
- Status: job open, identifiable and not already applied to, with a usable application destination.

Use `strong`, `possible` or `skip` with a reason. Proceed with strong matches under an apply mandate. Resolve material uncertainty before a consequential eligibility answer; never silently convert missing information into “No.”
