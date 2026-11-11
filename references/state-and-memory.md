# Private state and continuity

Keep memory in the user's private state directory, separate from exports and Git repositories. The default is `~/.local/share/job-application-assistant/`; reuse an existing location rather than creating competing trackers. Never commit resume PDFs, extracted resume text, contact details, compensation, disclosure answers, screenshots of private pages, OTPs, cookies or access tokens. Store secrets only through an appropriate credential mechanism, never in these files.

## Profile

Use `profile-template.json`. Each saved answer contains its value, source, confirmation date and scope. Sources can be a resume file/version or an explicit user answer. Keep unconfirmed fields absent or null. Preserve wording when it affects meaning: current fixed salary, total compensation and expected compensation are different fields, and currency and annual/monthly periods matter.

Separate durable facts (education, professional links) from preferences (locations, working hours) and changing facts (notice period, offers, compensation). Before reusing older or conflicting data, check whether it still applies. A user correction supersedes the old answer; retain a concise correction note where needed. Recompute experience from employment dates instead of indefinitely reusing “five years.” Do not convert total experience into equal experience in every skill. An explicit user-provided per-skill answer may be saved as such, with any material discrepancy clarified.

Sensitive demographics and disclosures are optional unless required for the specific application. Use only explicit user-provided answers, never inference from names, nationality, photos or other proxies. Do not assume a “No relationship” disclosure for one employer answers a different employer's question. Do not export these answers.

## Application queue

Use `applications-template.json`. Generate a stable local ID and deduplicate primarily by employer plus requisition ID, then canonical application URL and title/location. Store alternate source links. Separate a fit decision from application status.

Status vocabulary:

| Status | Meaning |
| --- | --- |
| discovered | Link captured; details not yet checked |
| shortlisted | Fit checked; ready to start |
| in_progress | Form or account work underway |
| awaiting_user | A specific answer, action or review is needed |
| draft_ready | Prepared for requested review; unsent/unsubmitted |
| submitted | Explicit success evidence recorded |
| submission_unconfirmed | Attempt made but success unclear; check before retry |
| blocked | Documented technical or access obstacle |
| skipped | User instruction, duplicate or poor fit; reason recorded |
| closed | No longer accepting applications |

For `submitted`, record confirmation text/status, time and a relevant receipt or page URL when available. Keep screenshots private if the tool requires proof. For `awaiting_user` or `blocked`, store the next action and whether form progress survives. Never count drafts, account creation or clicks as successful applications.

## Handoff and export

Update `handoff.md` with source coverage, completed totals, next eligible applications, pending user questions, browser/profile identity, important open-page URLs and private evidence paths. Do not store OTPs, passwords or authentication links. Reopen/rebind browser tabs using the current tool's documented discovery, not stale session IDs.

At the end, show submitted totals and a linked manual-follow-up list with reasons. If interrupted, resume from the queue and verify live state rather than resubmitting blindly. A skill is a reusable instruction package, not a running worker or scheduler.

When exporting or adding this skill to GitHub, package only the reusable skill folder, blank templates and generic references. Keep runtime state outside the package. Respect repository visibility preferences and inspect the exact staged/exported file list before publication.
