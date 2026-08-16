# Custom Instructions -- career-ops

<!-- ============================================================
     THIS FILE IS YOURS. It will NEVER be auto-updated.

     Put your own house rules, custom workflows, and automations
     here -- anything you want the agent to ALWAYS do (or never do).

     This is for PROCEDURAL rules ("HOW I want things done").
     For WHO you are (archetypes, narrative, comp, negotiation),
     use modes/_profile.md instead. Keeping the two separate keeps
     each one readable.

     The agent reads this file alongside the system instructions;
     your rules here take precedence over the defaults, as long as
     they don't break the Data Contract (your files are never
     touched, and we never auto-submit an application for you).

     Because this is a user-layer file, anything you write here
     survives `node update-system.mjs`. Put customizations HERE,
     not in CLAUDE.md / modes/_shared.md / other system files --
     those get overwritten on update.
     ============================================================ -->

## House Rules

<!-- Rules the agent should always follow. Examples:
     - Always write evaluation summaries in British English.
     - Never include a photo in my CV (US / ATS-first market).
     - Cap each batch run at 20 listings unless I say otherwise.
     - If a report scores below 6, skip the cover letter. -->
- Write every experience bullet in the XYZ formula — "Accomplished [X], as measured by [Y], by doing [Z]" — and never finalize a bullet that lacks a quantified Y (%, $, time, volume, scale). If no real number exists, use scope or frequency instead of inventing one; never fabricate a metric.
- 
- Start every bullet with a strong past-tense action verb (increased, built, reduced, launched, negotiated, automated). Never use "responsible for," "helped with," "worked on," "duties included," or passive phrasing.

- Cap each role to 3–6 bullets. Give the most recent and most relevant role the most bullets, and always put the single strongest, most quantified bullet first within each role — recruiters spend roughly 7 seconds on the initial screen and read in an F-pattern (title → company → dates → top lines), so front-loaded impact matters most.

- Enforce a strict one-page limit for cv generation.
 
- Use a single-column, reverse-chronological layout only. Never use tables, text boxes, multi-column layouts, sidebars, or graphics (including skill-rating bars or stars) — ATS parsers read linearly and will scramble, skip, or drop content placed in these elements.

- Use only standard section headings: "Experience," "Education," "Skills," "Projects." Never rename them creatively — ATS categorization depends on recognizing these exact labels.

- Never place name, contact info, or any content that must be parsed inside a document header or footer — many ATS scrapers ignore that layer entirely.

- Never use icons for phone/email/LinkedIn — use plain text labels instead.

- Default to producing a text-based, selectable PDF.

- Use consistent MM/YYYY date formatting throughout the whole resume.

- Before drafting or evaluating any resume, pull the job description first and mirror its exact keyword phrasing (skill names, tool names, tech stack) in the skills section and bullets, without keyword-stuffing. Never swap in a generic synonym for a term the JD uses explicitly (keep "Python," don't write "programming languages").

- Always tailor the summary and skills section per company and role. Never reuse one generic resume version across different companies or postings.

- When the target company is Amazon, tag at least one bullet to a Leadership Principle emphasized in that JD (commonly Customer Obsession, Ownership, Bias for Action, Deliver Results, Dive Deep) and note which LP each mapped bullet demonstrates for the candidate's reference.

- Default to the XYZ phrasing as close to verbatim as the bullet allows. Accomplished [X], as measured by [Y], by doing [Z]. 

  example: "Increased signup conversion 22% by redesigning the onboarding flow to cut form fields from 12 to 4"
  X = increased signup conversion, Y = 22%, Z = redesigning the onboarding flow. You could also lead with Z if the method is the more impressive/relevant part for that job:
  "Redesigned the onboarding flow, cutting form fields from 12 to 4, which increased signup conversion 22%"

- Never include a photo, an objective statement, or first-person pronouns (I, my, me) anywhere on the resume.

- 3 Bullet points per role, with the most relevant/impactful one first.

- Professional summary should be written in a way that exactly matches what the JD is asking for.

- Drop the Core Competencies grid so that the resume fits on one page. Never include a `competencies` key in any CV payload — omit it entirely so the section never renders (the pipeline strips it automatically as a safety net, but it should never be generated in the first place). 

<!--(none yet -- add yours above)-->

## Custom Workflows

<!-- Multi-step routines you run often, given a short name. Examples:
     - "weekly review": scan my saved portals, evaluate the new roles,
       then give me a one-paragraph summary of the top 3.
     - "prep <company>": pull the JD, generate STAR stories from
       article-digest.md, and draft 5 likely interview questions. -->

<!--(none yet -- add yours above)-->

## Output Preferences

<!-- How you like results formatted. Examples:
     - Reports: lead with the score and the one-line verdict.
     - Show the per-step token breakdown after a batch run.
     - Save PDFs date-first: YYYY-MM-DD-company.pdf -->

- Save PDFs like company.pdf, You don't need to save date in the file name.

<!--(none yet -- add yours above)-->

## Off-Limits

<!-- Things the agent must never do for you. Examples:
     - Never auto-fill or submit an application without showing me first.
     - Never edit a system file to customize my setup -- put it here. -->

<!--(none yet -- add yours above)-->
