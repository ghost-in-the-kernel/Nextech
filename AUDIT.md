# What is wrong with `www.nextech.com`

Read on 2026-11-06: 82 pages of `https://www.nextech.com`, in a real browser, logged out, one page at a time. Nothing was sent, bought or signed in to.

## Links that need a look (2)

Each of these links answered an error or did not answer. A person is to look at every one, whatever the site means by it: nothing here is cleared by a rule. A link leaves this list only when the team lists it, with the status it answers, in the suite's expected-links block.

- `https://imimobile.com/` its name no longer resolves: the site is gone; linked from /partnerships; broken (SITE-33)
- `https://qpp.cms.gov/mips/explore-mips-value-pathways?py=2025` answered 404; linked from /blog/mips-value-pathways; broken (SITE-33)

Found **3 major** and **5 minor**.

## major SITE-08 10 form fields on 5 pages have no label

**Why it matters.** A screen reader announces a field with no label as "edit text", so a blind visitor cannot tell what to type; a placeholder alone vanishes once typing starts. Accessibility audits fail it.

**Likely fix.** Give each field a \<label for="its id"\> \(each id used once on the page\), or an aria-label.

<details open>
<summary>5 pages</summary>

- `/solutions/ai` 2 fields: \`\<select name="specialty"\>\`, \`\<select name="state"\>\`
- `/products/cora` 2 fields: \`\<select name="specialty"\>\`, \`\<select name="state"\>\`
- `/request-demo` 2 fields: \`\<select name="specialty"\>\`, \`\<select name="state"\>\`
- `/specialties/ophthalmology/crm-software` 2 fields: \`\<select name="specialty"\>\`, \`\<select name="state"\>\`
- `/request-info` 2 fields: \`\<select name="specialty"\>\`, \`\<select name="state"\>\`

</details>

## major SITE-33 2 links to other sites lead nowhere: the pages are gone

**Why it matters.** Sites move and close: a visitor who follows one of these links meets an error page, or nothing at all, on someone else's site, and leaves thinking less of this one.

**Likely fix.** Point each link at where the page lives now, or take it out. The suite's link report asks every one again on each run, and fails when one that answered stops.

<details open>
<summary>2 pages</summary>

- `https://imimobile.com/` its name no longer resolves: the site is gone; linked from /partnerships
- `https://qpp.cms.gov/mips/explore-mips-value-pathways?py=2025` answered 404; linked from /blog/mips-value-pathways

</details>

## major SITE-21 The site's own scripts throw 4 errors on 2 pages

**Why it matters.** An error nothing catches stops the script that threw it: whatever it was doing \(a form's checks, a cart, tracking\) is left undone. Visitors never report it; it is seen only in the browser's console.

**Likely fix.** Open the page with the browser's developer tools, read the console, and fix each error at the line it names.

<details open>
<summary>2 pages</summary>

- `/aesthetically-speaking` 2 errors: A network error occurred. and 1 more
- `/blog/how-to-transition-from-paper-charting-to-ehr-in-6-steps-saving-your-practice-time-and-money` 2 errors: A network error occurred. and 1 more

</details>

## minor SITE-16 67 links on 37 pages point to a part of the page that is not there

**Why it matters.** A visitor clicks and nothing happens: the link names a \#part no element on the page has.

**Likely fix.** Give the part it means the id the link names, or point the link at the right one.

<details>
<summary>37 pages</summary>

- `/blog/healthcare-cybersecurity-challenges` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-to-get-patient-referrals` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/cloud-based-ehr` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/aesthetically-speaking` 1 link: \`\<a href="\#play"\>\`
- `/press-releases/connected-innovation-and-specialty-specific-ai-take-center-stage-at-nextech-edge-2026` 1 link: \`\<a href="\#share"\>\`
- `/industry-news/nextech-launches-clinical-assistant-unlike-generic-bolt-on-scribes` 1 link: \`\<a href="\#share"\>\`
- `/press-releases/nextech-reduces-healthcares-payment-reconciliation-burden-with-updated-embedded-payment-processing-platform` 1 link: \`\<a href="\#share"\>\`
- `/industry-news/nextech-rolls-out-ai-scribe-built-for-specialty-physician-practices` 1 link: \`\<a href="\#share"\>\`
- `/press-releases/nextech-unveils-agentic-ai-capabilities-for-patient-experience-through-new-partnerships` 1 link: \`\<a href="\#share"\>\`
- `/industry-news/nextech-cio-ciso-shares-perspective-on-phishing-threats-in-healthcare-0` 1 link: \`\<a href="\#share"\>\`
- `/blog/ehr-or-pm-how-having-both-can-help-your-practices-bottom-line-nextech` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/mips` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/mips-value-pathways` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-to-transition-from-paper-charting-to-ehr-in-6-steps-saving-your-practice-time-and-money` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/ophthalmology-abbreviations` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/7-social-media-strategies-for-aesthetic-practices-and-med-spas` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/iv-therapy-laws-by-state` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/ehr-vs-emr` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/cost-of-not-switching-plastic-surgery-software` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/stop-leading-with-price-in-financing-conversations` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/healthcare-financial-management` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/celebrating-career-journeys-marian-llamas` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/ehr-for-small-practices` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/med-spa-laws-by-state` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/patient-engagement-in-healthcare` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/cost-and-roi-of-ehrs` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/survey-50-of-physicians-havent-heard-of-macra` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/fresh-perspectives-nextech-celebrates-national-intern-day` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-to-prevent-healthcare-data-breaches` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-to-maximize-reimbursements-at-your-practice` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-to-address-and-prevent-pa-burnout` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/how-providers-safeguard-their-revenue-cycle` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/benefits-of-chatbots-in-healthcare` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/ophthalmology-cpt-codes` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/net-vs-gross-collection-rates` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/coding-telehealth-visits` 2 links: \`\<a href="\#share"\>\` and 1 more
- `/blog/what-is-pecos` 2 links: \`\<a href="\#share"\>\` and 1 more

</details>

## minor SITE-03 18 of the site's own links redirect before they arrive

**Why it matters.** Every click on one of these links costs an extra round trip before the page starts loading, and search engines see one page at two addresses.

**Likely fix.** Link to each page's final address \(with or without its trailing slash, as the server serves it\).

<details>
<summary>18 pages</summary>

- `/case-study/ophthalmology-associates-of-fort-worth/` 301, 301 to /case-studies/ophthalmology-associates-of-fort-worth
- `/case-study/short-hills-ophthalmology-group` 301 to /case-studies/short-hills-ophthalmology-group
- `/21st-century-cures-act` 301 to /
- `/medspa` 301 to /specialties/med-spa
- `/advanced-analytics` 301 to /solutions/advanced-analytics
- `/case-study/loden-vision` 301 to /case-studies/loden-vision
- `/dermatology/ehr-pm-software` 301 to /specialties/dermatology/ehr-software
- `/ophthalmology/ehr-pm-software` 301 to /specialties/ophthalmology/ehr-software
- `/plastic-surgery/ehr-pm-software` 301 to /specialties/plastic-surgery/ehr-software
- `/orthopedic/ehr-pm-software` 301 to /products/ehr
- `/about` 301 to /company/about
- `/blog/get-to-know-nextech-and-our-newest-feature-updates` 301 to /resource-center
- `/thrive` 301 to /products/consulting
- `/touchmd` 301 to /products/touchmd
- `/cloud-based-ehr` 301 to /products/ehr
- `/plastic-surgery/case-study/davinci-plastic-surgery` 301 to /resource-center
- `/dermatology/case-study/the-herschthal-practice` 301 to /resource-center
- `/careers` 301 to /company/careers

</details>

## minor SITE-17 3 pages have no description for search results

**Why it matters.** Search results show the description under the title; without one, the search engine picks a line of the page, often the menu or a cookie notice.

**Likely fix.** Give each page a \<meta name="description"\> of a sentence or two saying what it offers.

<details open>
<summary>3 pages</summary>

- `/author/nextech` no meta description
- `/author/david-slazyk` no meta description
- `/author/tom-robinette` no meta description

</details>

## minor SITE-24 3 security headers no page sends

**Why it matters.** Each header closes a door attackers use \(a downgrade to http, a script slipped in, the site framed in another to trick a click\). Security reviews and compliance checklists ask for them, and they cost a line of server configuration.

**Likely fix.** Add the missing headers in the web server or the CDN \(one setting each\), starting with Strict-Transport-Security.

<details open>
<summary>3 pages</summary>

- `/` no page of the site sends Content-Security-Policy \(which scripts may run\)
- `/` no page of the site sends X-Frame-Options or frame-ancestors \(another site cannot frame it to trick a click\)
- `/` no page of the site sends X-Content-Type-Options: nosniff

</details>

## minor SITE-18 1 address goes through a chain of redirects

**Why it matters.** Each redirect is another round trip before the page starts to load, and search engines may give up on a long chain.

**Likely fix.** Redirect each old address straight to the final one, and link to the final address.

<details open>
<summary>1 page</summary>

- `/case-studies/ophthalmology-associates-of-fort-worth` /case-study/ophthalmology-associates-of-fort-worth/ → /case-study/ophthalmology-associates-of-fort-worth → /case-studies/ophthalmology-associates-of-fort-worth \(301, 301\)

</details>

Found by Suite Builder's crawler, which identifies itself in its User-Agent and obeys robots.txt. A major finding lets a visitor or a search engine down now; a minor one is worth fixing. Each lists every page the crawl saw it on; the crawl reads a sample of a big site, so a finding can reach further than it lists.
