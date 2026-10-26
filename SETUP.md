# South Carolina site setup

This site was cloned from the Georgia site (Peak 301 Pros GA) and made specific to South Carolina.

## Before the partner login and job form work
Set these in Netlify (Site configuration > Environment variables). They are secrets and are never stored in this repo:

- PORTAL_SESSION_SECRET: a long random string
- PORTAL_ADMIN_CODE: the admin access code for this site
- PORTAL_ACCOUNTS: the partner list, as a JSON list of {key,name,prefix,contact,code}
- JOBNIMBUS_API_KEY and JOBNIMBUS_WRITE_KEY: from the Peak 301 Pros JobNimbus account (NOT Go Dawgs Roof Roof's)
- PORTAL_OFFICE_USER_ID and PORTAL_PRODUCTION_USER_ID (optional): JobNimbus user ids that receive the office and production tasks; tasks are skipped if unset
- PORTAL_PIPELINE_ON=1 (optional): turns on the automatic job-status mover. It is off until set
- PORTAL_APPLICATOR_NAME (optional): name printed on warranty letters (default: Peak 301 Pros South Carolina)

Until these are set, the public marketing page works but partner sign-in will not.

## Pricing
Partner pricing is not published on any public page. Share the partner rate sheet with approved partners only.

## Open items
- Confirm the contact email and phone shown on the page (partners@peakprossc.com).
- The back-end functions still use Georgia's GDRR workflow (JobNimbus statuses, estimate templates, warranty letter). Review before pointing real South Carolina jobs at them.
