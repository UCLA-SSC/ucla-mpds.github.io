# MPDS website: final pages reference

**Last updated:** October 23, 2026, about 3:15 pm (Pacific). Draft v6 is current. Draft v5 was soft-launched on Oct 23 and must not be edited.
**Purpose:** the starting point for any Claude session that works on the MPDS (Master of Population Data Science) recruitment website. Read this first. Update it (the "Change log" and any affected section) every time the website changes.

---

## 1. Where the final website lives

| What | Where |
|---|---|
| **Final pages (source of truth)** | Box › CCPR.MPDS › Website › **Draft v6** (on Martha's computer: `C:\Users\Martha\Box\CCPR.MPDS\Website\Draft v6\`) |
| Copy source (all page text) | Google Doc "MPDS Website Page Text": https://docs.google.com/document/d/1G60GtqwrL4u4MNV5vEkp-8Oks6eyKJjUeAnkYLRmVl8/edit |
| Cost sheet source | Google Doc "MPDS Cost Sheet, Fall 2027 (draft)": https://docs.google.com/document/d/1RqWF7Gd7M1oDqWXlMlnmg5IpbnEhoZsxUE5UVXdJX18/edit (older 1-page content; the PDF in Draft v6 is the current 2-page version) |
| ROI method source | Google Doc "MPDS ROI Methodology (draft)": https://docs.google.com/document/d/1hsZ4zfZ9_5FigLCy3hynlgIsC2G8qr8-OGY4zTbGLyE/edit |
| Copy doc snapshot | `Draft v6/MPDS Website Page Text.docx`: Word export of the Google Doc (with its comments) as of Oct 22, ~5:10 pm. The Google Doc stays the live source. |
| Earlier drafts | Box › Website › Draft v5 (soft-launched Oct 23), Draft v4, Draft v3, Draft v2, Drafts. Do not edit these. |

### Contents of Draft v6
```
Draft v6/
├── index.html                        (the Home page; every page's logo links here)
├── Home.html                         (redirect only: sends old Home.html links to index.html; do not edit)
├── Faculty.html
├── Program.html
├── Tuition-and-Aid.html
├── Admissions.html
├── MPDS-Cost-Sheet-Fall-2027.pdf     (2 pages; linked from Tuition & Aid)
├── MPDS-ROI-Methodology.pdf          (linked from Tuition & Aid "How we calculate ROI (PDF)")
├── MPDS Website Page Text.docx       (Word snapshot of the copy doc)
├── MPDS website - final pages reference.md   (this file)
└── images/
    ├── favicon-32.png, apple-touch-icon.png   (browser-tab and phone icons: UCLA wordmark on UCLA Darkest Blue)
    ├── *-800.webp, *-1600.webp, *-1600.jpg   (web-optimized photos used by the pages)
    ├── mpds-logo-white.svg           (approved official "Unboxed White" wide lockup, version C, trimmed; header at 513×42)
    ├── faculty-*.jpg                 (10 headshots from the trifold brochure, 300×300)
    ├── mpds-logo-white.png           (old PNG logo, no longer used)
    ├── mpds-logo-stacked-white.png
    ├── lifem-network.jpg             (hero network background)
    ├── botanical-garden-students.jpg, bruin-walk.jpg, go-bruins-sunset.jpg,
    ├── research-poster.jpg, royce-arcade.jpg, royce-hall-dusk.jpg, seminar-room.jpg
```
Each page is one self-contained HTML file (inline CSS, no build step). Pages link to each other by relative file name, so the folder works as is.

### Preview pages (claude.ai artifacts)
Each preview holds all four pages plus the images and PDFs; they differ only in which page opens first. They match Draft v6, except that in the previews the logo links to Home.html (a preview cannot hold its own index.html); the Box files link to index.html.
- MPDS Home Page: https://claude.ai/artifact/A9YQDD7NurksSLKxsGdbVe
- MPDS Program Page: https://claude.ai/artifact/D4mZvVm3uYGDC1AnWE15jL
- MPDS Tuition and Aid Page: https://claude.ai/artifact/EDxtC9Udrw6uiAPumV9byV
- MPDS Admissions Page: https://claude.ai/artifact/QQcdhcSng13PVDLZmZ8bbs
- MPDS Faculty Page: https://claude.ai/artifact/PLqC7nFzp64QcsaaG9s1du (added Oct 23; private until shared; declares `downloads`)

---

## 2. The rule for changes

1. **The Google Doc is the copy source.** Martha edits text there; the pages are updated to match word for word (text only, not formatting). Any text change made on the page side is carried back into the doc.
2. **Every change goes to all of these, every time:**
   - the page file in Box › Website › Draft v6 (for Home, edit index.html);
   - all four preview artifacts (each one contains every page);
   - this reference file (Change log, plus any section it affects).
3. **Comparing doc and pages:** compare paragraph by paragraph. The doc's comment threads start at the line beginning "[a]Notes:"; leave them out. Expected noise when extracting text: big numbers glued to their labels in "At a glance" tiles, step numbers (01, 02…), the path grid's column labels, and the ROI chart rows (hidden from screen readers on the page; the chart's description is in its aria-label).
4. **More than one Claude session may edit these pages.** Before editing, re-read the current Draft v6 file (or the preview's published file) and build on it.

---

## 3. Site map and page content

**Menu (all pages):** The Program · Meet the Faculty · Admissions · Tuition & Aid · Apply to MPDS (goes to Admissions.html#how).
**Small gold labels** (hero eyebrows and "At a glance"): 14px, spaced capitals (letter-spacing 0.12em, CSS uppercase), as in the brochure. Note: UCLA web guidelines discourage all caps; this was Martha's choice (Oct 23).
**At a glance rows** (Home, Program, Tuition): brochure style: gold figures (52px number + 30px unit, e.g. "15 courses"), 17px white description, thin rules above and below and between tiles.
**Footer (all pages):** mpds@ccpr.ucla.edu (mailto), UCLA accessibility, terms of use, nondiscrimination.
**Application links:** "Start your application" and "Apply through UCLA Division of Graduate Education" go to https://apply.grad.ucla.edu/portal/landing.

### Home (`Home.html`)
Sections: hero · At a glance · What is population data science? · Why MPDS? (cards 01–03) · Who should apply? · Questions about the program? (info session and contact).

### The Program (`Program.html`)
Sections: hero · **At a glance** (3 tiles: #1 U.S. public university / U.S. News & World Report, 2027; 15 courses over 6 quarters (20 months), with an accelerated 16-month option; Jan. 15 priority deadline / Final deadline: June 30, 2027) · **Why UCLA?** · **What you'll study** (6 cards: Social Science, Data Science, Professional Skills, Data Science in Action, Mentored Capstone Project, Choose from 40+ UCLA Electives) · **Your path through the program** (grid) · Program FAQs · Questions about the program?
- Path grid: course titles in sentence case with "&"; units inline after "·". Year 1 "Foundations": Social & population science; Statistical analysis & data science 1 and 2; Programming, AI, data management & visualization; Elective in social or data science; Data science in action; summer "Optional internship". Year 2 "Applications": Elective in social science; Elective in statistics & data science; Communication, collaboration & presentation; yellow box "Data science in action / 2 units each quarter · fall through spring"; Capstone project with a faculty mentor.
- Grid note (one paragraph): "Shaded boxes with dashed outlines are electives, chosen from more than 40 graduate (incl. PhD) courses in demography, economics, geography, public health, political science, sociology, and statistics and data science. Summer internships require enrollment in a one-unit summer course. International students must obtain Curricular Practical Training (CPT) authorization in accordance with federal requirements."

### Meet the Faculty (`Faculty.html`, added Oct 23)
Hero (eyebrow "Faculty"; H1 "Learn from renowned faculty"; brochure text "You'll study in person with leading scholars in economics, epidemiology, geography, political science, public health, sociology, statistics, and data science. Faculty are selected for their excellent teaching and mentoring records.") · **Our core faculty include:** circle headshots only (no cards), gold name, field below: Martha Bailey (*Program Director*, Economics, Demography); Onyebuchi Arah (Epidemiology, Statistics); Hiram Beltrán-Sánchez (Demography); Jennie Brand (Sociology, Statistics); Chad Hazlett (Statistics, Political Science); Patrick Heuveline (Demography, Sociology); Juliana Londoño Vélez (Economics); Ian Lundberg (Sociology); Ann Owens (Sociology); Naomi Sugie (Sociology) · Questions about the program? (Zoom + Explore the program). "Meet the faculty" links on Home and Program go here.

### Tuition & Aid (`Tuition-and-Aid.html`)
Sections: hero · **At a glance** (3 tiles: "$64,800 / tuition for the full program + fees and health insurance" with a gold "Cost sheet (PDF)" link; "8-34% / projected annual return on investment"; "100% / of applicants considered for merit fellowships, with no separate application") · **A degree that pays for itself** (ROI chart by bachelor's field: Sociology 16–34%, Public Health 12–29%, Geography 10–27%, Economics 8–24%; source note; "How we calculate ROI (PDF)") · **Tuition and fees** ($1,350/unit, $32,400/year, $64,800 tuition; estimated total about $84,000; "Download the cost sheet (PDF)") · **Ways to pay for your degree** (4 cards) · Cost and financial aid FAQs · Questions about cost?
- Ways to pay cards:
  - 01 Merit fellowships: "We automatically consider every applicant for merit-based fellowships, and many receive them. No separate application is needed. The program will contact recipients."
  - 02 Financial aid: "UCLA offers a variety of financial aid resources and tools for students. Visit the UCLA Division of Graduate Education financial aid page for details."
  - 03 Employer support: "Many employers help pay for graduate study. If yours needs documents for internal approval, such as a program description, cost estimate, or enrollment letter, write to us." ("write to us" is a mailto link to mpds@ccpr.ucla.edu)
  - 04 Veterans: "…contact UCLA's School Certifying Official… Visit this website for details." (links to the Chapter 33 Post-9/11 GI Bill page)
- ROI basis: MPDS expected earnings $100,000–$135,000; program cost $83,718; 20 months of forgone salary. The headline figure is written "8-34%" with a hyphen.

### Admissions (`Admissions.html`)
Sections: hero (with "Start your application"; no info-session link) · Key dates (Jan. 15, 2027 priority deadline with decisions by March 1; June 30, 2027 final deadline; Fall 2027 first cohort) · Who should apply? · What to submit · How to apply · English proficiency and international applicants · Admissions FAQs · Questions about applying?
- Deadline FAQ ends "…and applications received after January 15 will be reviewed on a rolling basis."

---

## 4. Design system (as built)

- **UCLA brand colors:** UCLA Blue `#2774AE`, Darkest Blue `#003B5C` (header/page fields), Darker Blue `#005587` (links on light), UCLA Gold `#FFB81C` (accents, buttons, section rules, gold links), white text on blue fields; body text on light `#1B2A35`, muted `#4A5A66`, light blue fills `#DAEBFE`.
- **Type:** 'Helvetica Neue', Helvetica, Arial, Roboto, sans-serif (UCLA web fallback stack).
- **Header logo:** `images/mpds-logo-white.svg` (approved version C, white) at a fixed 513×42 px; it never shrinks horizontally. At widths ≤1120px the header wraps to two rows; at ≤560px the logo scales to the screen width.
- **Inner-page heroes:** 640px tall over the LIFE-M network background (opacity 0.62); Home keeps a stronger splash network.
- **Buttons:** gold fill `#FFB81C` with `#003B5C` bold text. FAQs are fold-out (details/summary) on the three inner pages. "What to submit" item titles on Admissions are dark gold.
- **Section heading pattern:** 56×3px gold rule above a 44px light-weight h2.

- **Content source for facts:** MPDS proposal, November 3, 2025 (`CCPR_SSGPDP_Proposal_Nov.3.2025_final.pdf` in this project): curriculum, units, timeline, tuition estimate.

### Cost figures behind the pages (fall 2027 entrants, UCLA 2026–27 fees)
| Item | Per year | Full program (20 months) |
|---|---|---|
| Tuition ($1,350/unit × 24 units/year; same for residents and non-residents) | $32,400 | $64,800 |
| Campus fees (year 1 includes a one-time $94.43 document fee) | $1,988.91 (yr 1), $1,894.48 (yr 2) | $3,883 |
| UC Student Health Insurance Plan (UCSHIP), waivable with comparable coverage | $7,517.28 | $15,035 |
| **Estimated total** | | **$83,718** (about $84,000) |

Fee items per year: Student Services $1,344.00; Ackerman $81.00; GSA $38.25; Writing Center $23.16; SPARC $150.00; Seismic $113.00; Wooden $45.00; BruinGo $36.39; BruinFresh $15.00; GOLD $41.68 (estimated); UCGPC $7.00 (modeled on UCLA MQE and MASDS cost-of-attendance pages).

### UCLA web compliance rules followed
16px minimum body text; 12.8px minimum captions; no all-caps; left-aligned text; AA color contrast; descriptive link text; nav as a list in `<nav>`; one `<h1>` per page; 44px minimum touch targets; alt text under 125 characters on every non-decorative image; skip-to-content link; accessibility, terms of use and nondiscrimination links in the footer. Only the UCLA web font stack (no webfonts; serif headlines need approval from UCLA Strategic Communications). UCLA Gold #FFD100 is not used; Darkest Gold #FFB81C is.

---

## 5. Technical notes for Claude

- **Preview artifact wrapper:** each preview's `index.html` starts with a short wrapper skeleton followed by the full page. CSS added inside the first `</style>` (the wrapper's) is stripped on publish; page CSS must go in the page's own `<style>` (the second `</style>`).
- **Publishing a page change to the previews:** publish with the preview's `url`, its index file as `file_path`, and the changed page in `files` (e.g. `{"Tuition-and-Aid.html": "Tuition-and-Aid.html"}`) from a folder holding that preview's files. If the publish is refused because the published file wasn't read in this session, read it (`action: read`, `path`), confirm it matches your base, then publish again.
- **PDF downloads in previews:** Program and Tuition & Aid carry a small script that makes PDF links download inside the claude.ai preview (the previews declare the "downloads" capability). Keep it when merging; it does nothing on a normal web server.
- **Saving to Box (through the desktop app):** stage the file from a brand-new output folder each time (reusing a staged path can silently save an older copy), commit it to `...\Website\Draft v6\<file>`, and then list the folder to check file sizes.
- **Google Doc edits:** `replaceAllText` for wording swaps; positional inserts and deletes need a fresh `read_doc` revision ID. Exporting HTML with "$…$" in one paragraph can turn into an equation in Docs.

---

## 6. Open items

**Main remaining update: the Zoom info-session link.**
- "Register" / "Register for a Zoom info session" buttons on Home (2), Program and Admissions still point to "#". Waiting on a webinar-compliant Zoom account; once Martha has the webinar registration link, wire all four buttons to it and fill in the Home card's session date and time.

Smaller items (lower priority):
- Add Google Analytics (GA4) once the live address is set up (item 31).
- Martha to confirm the live address is https://mpds.ss.ucla.edu/ (the cost sheet PDF also prints www.mpds.ss.ucla.edu). The link-preview tags (og:url, og:image) on every page use it; change them if the address differs.

### Before public launch (carried over from earlier notes)
- Check usage rights for every photo in `images/` against the 9/29 and 10/6 contact sheets (project files). Some are marked "No Advertising": fine on the website, not in paid ads.
- Confirm the license for the LIFE-M network background (from life-m.org).
- WebAIM contrast check: on Oct 17, gold eyebrows and subheadlines measured about 2.6–4.2:1 where bright network nodes pass behind them (AA needs 4.5:1); a soft darkening behind the text block fixes it.
- Confirm the "U.S. News & World Report, 2027" citation year and the Lightcast source wording for the ROI figures.

---

## 7. Change log (newest first)

- **2026-10-23, ~3:05 pm (second sync):** Program At a glance synced to Martha's doc edits: "over 6 quarters (20 months), with an accelerated 4-quarter option" and date "January 15" (no year; tile back to one line). Note: Home, the Program path note and the Program FAQ still say "16-month".

- **2026-10-23, ~3:15 pm:** Synced Martha's doc edits: Program At a glance now "January 15, 2027" / "priority deadline, with decisions by March 1; rolling decisions after" (the doc had a date chip reading "Jan 15, 2026"; replaced with text "January 15, 2027"); Tuition At a glance "$64,800 / tuition + fees, health insurance, materials & personal expenses" and "100% / applicants considered for merit fellowships, no separate application". Added "Calculate ROI (PDF)" link under 8-34% (links to MPDS-ROI-Methodology.pdf; same style as "Cost sheet (PDF)"), also added to the doc. Layout fix on all pages: the hero now grows when its text needs more room (it overlapped At a glance at about 1000–1300 px wide, also in the soft-launched v5), and the menu drops below the logo up to 1260 px (it ran off the right edge at 1121–1240 px).

- **2026-10-23, ~3:05 pm:** "Jan. 15" spelled out as "January 15" everywhere (Google Doc: 4 places; Admissions and Program pages in Draft v6 and previews). Admissions Key dates numbers now shrink slightly on phones (clamp 34–48px) so "January 15, 2027" stays on one line. "Jan. 21, 2026" (TOEFL scoring date) left as is.

- **2026-10-23, ~3:00 pm:** Item 21 settled. The list of costs left out of the estimates is now "materials, housing, and personal expenses" everywhere: Tuition and fees paragraph (unchanged), Tuition FAQ now "Materials (e.g., computer, software, books), housing, and personal expenses." (Google Doc, Draft v6, previews), and the cost sheet PDF note now "Estimates do not include materials, housing, or personal expenses." (Draft v6 and previews).

- **2026-10-23, ~2:45 pm:** Draft v5 soft-launched; Draft v6 created as the new working copy (all v5 files). In v6 the header logo on every page links to index.html; Home.html is now a redirect to index.html. Martha confirmed the studentaid.gov links work.

- **2026-10-23, afternoon:** Applied Martha's numbered pre-launch list (items 1–6, 12–20, 22–30; items 7–11 dropped) in the Google Doc and all five pages. Highlights: Admissions transcript FAQs now use UCLA's "you will be contacted" language and send official records to Attn: MPDS, CCPR, 4284 Public Affairs Bldg., Box 957236, Los Angeles, CA 90095; priority deadline Jan. 15, 2027 with rolling review after; federal loan FAQ rewritten (8.07%, 1.057% fee, tiered standard plan or RAP); STEM OPT, GI Bill, FAFSA, Financial Aid, UCSHIP and StudentAid.gov links added; every email address is now a mailto link; electives listed alphabetically; "Data Science in Action" grid label; Home h1 period removed. Added favicon, phone icon, page descriptions and link-preview (Open Graph) tags to every page, and index.html (copy of Home) to Draft v5.

- **2026-10-23, ~1:50 pm:** Tuition & Aid "Write to us" button now opens an email to mpds@ccpr.ucla.edu. Pre-launch review done (typos, consistency, links); Martha is publishing quietly to test; Zoom/info-session placeholders stay until the webinar link arrives next week.
- **2026-10-23, ~1:05 pm:** Each faculty name on the Faculty page (and in the copy doc) links to their official UCLA page, opening in a new tab: Bailey economics.ucla.edu/person/martha-bailey; Arah and Beltrán-Sánchez ph.ucla.edu faculty-staff-directory; Brand soc.ucla.edu/person/jennie-e-brand; Hazlett polisci.ucla.edu/person/chad-hazlett; Heuveline, Lundberg, Owens, Sugie soc.ucla.edu/person/…; Londoño Vélez economics.ucla.edu/person/juliana-londono-velez.
- **2026-10-23, ~1:00 pm (from Martha's doc edits):** Faculty page: "Our distinguished community has:"; grid heading now "Our core faculty" with a new paragraph ("MPDS’s internationally acclaimed faculty come from across the university, with fields in demography, economics, geography, political science, public health, and sociology. Faculty are selected for their excellent teaching and mentoring records."); Martha Bailey's fields "Economics, Demography". Doc and all five pages match word for word.
- **2026-10-23, ~1:00 pm (faster photos):** All seven site photos now load web-optimized versions: `images/<name>-800.webp` and `-1600.webp` (served by screen size through `srcset`/`sizes`), with `-1600.jpg` as the fallback `src`. The top photo on each page has `fetchpriority="high"`; lower photos use `loading="lazy"`. Photo download per page dropped about 70% (Home ≈2 MB → 596 KB). Copies saved under new names in Box › Website › Contact sheets › Web-optimized (`<original name>_web-800.webp`, `_web-1600.webp`, `_web-1600.jpg`). The old 2,400px JPEGs (`images/<name>.jpg`) are no longer used by the pages. To add a new photo: make 800 and 1600px WebP plus a 1600px JPEG, and use the same `srcset` pattern.
- **2026-10-23, ~12:50 pm:** Hero photos swapped: Faculty page now uses `royce-hall-dusk.jpg` (Royce Hall and downtown LA at dusk); Tuition & Aid ("Invest in your future") now uses `royce-arcade.jpg` (three students walking under the Royce Hall arches; the same photo also appears in Home card 03).
- **2026-10-23, ~12:45 pm:** "Why UCLA?" (with its four bullets) moved from the Program page to the Faculty page, between the hero and "Our core faculty include:"; copy doc moved to match. New fifth preview, MPDS Faculty Page. Full word-for-word check: doc and all five pages match.
- **2026-10-23, ~12:40 pm:** Headshots for Arah, Beltrán-Sánchez, Hazlett and Sugie recropped from the originals (Downloads › CCPR.MPDS › Webpage › Headshots) so the whole head fits in the circle, with a little blurred background added above where the original was tight; Heuveline's headshot added (cropped from PH.png; photo credit: Oliver Chien/UCLA International Institute).
- **2026-10-23, ~12:35 pm:** Faculty page and copy doc: Patrick Heuveline (Demography, Sociology) replaces Adriana Lleras-Muney, in alphabetical order between Hazlett and Londoño Vélez. Needs a headshot (`images/faculty-heuveline.jpg`).
- **2026-10-23, ~12:15 pm (brochure alignment):** New Meet the Faculty page and menu tab (brochure text and headshots; circle headshots only); "Meet our team" links renamed "Meet the faculty". Approved SVG logo (version C) in the header. All photos replaced with full-resolution originals from Box › Website › Contact sheets (2400px wide, sRGB). At a glance restyled to the brochure; small gold labels in spaced capitals. Program: eyebrow "The Program"; "Why UCLA?" rewritten from the brochure with bullets (17 Nobel laureates; 41 MacArthur Fellows; 12 National Medal of Science recipients; $1.6 billion in annual research funding); cards 01–03 put units/courses on a second line; card 05 "6 units (9 months)". Wording from the brochure: "STEM-designated"; "#1" not "No. 1"; Why MPDS ("The hard part is knowing which questions are worth asking and how well the data can answer them." + "teaches you to use data carefully and thoughtfully"); shorter Who should apply?; capstone "and a faculty mentor"; Admissions key date "…; rolling decisions after". Copy doc updated to match (new Faculty Page section).
- **2026-10-22, ~5:15 pm:** Word snapshot of the copy doc saved to Draft v5. Older Claude notes in the project (Oct 17 handoff, Oct 18 "what we learned", harmonization notes) retired; their still-useful content moved into this file.
- **2026-10-22, ~5:10 pm:** All four final pages resaved to Draft v5 (Home 22,366; Program 37,090; Tuition-and-Aid 35,459; Admissions 37,243 bytes). Zoom webinar link marked as the main remaining update.
- **2026-10-22, ~5:10 pm:** Tuition & Aid At a glance: "Cost sheet (PDF)" link is now gold; tile text now "tuition for the full program + fees and health insurance" (from the doc). Saved to Draft v5 and all previews.
- **2026-10-22, ~5:05 pm:** Draft v5 created in Box (final pages, images, cost sheet, ROI PDF).
- **2026-10-22, ~5:00 pm:** Program "Why UCLA?" ends "…universities—all in Los Angeles…". Tuition card 01 and 03 wording per the doc (see section 3).
- **2026-10-22, ~4:55 pm:** Doc synced to pages word for word (U.S. News citation added; grid note joined into one paragraph; "Attend an info session" removed from the doc).
- **2026-10-22, earlier:** Path grid in sentence case with "&", units inline; info-session tab and links removed; long logo restored with a fixed width; Program restructured to six cards plus "Why UCLA?" (capstone section removed).
