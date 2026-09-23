# Recraft CTA message-match brief (as of this run)

**PR:** (this PR) (branch `cta-scout/pm-message-match`, open, NOT merged — for human review)

## TL;DR
- **What changed since the last run (earlier today):** the Meta creatives are the same (22 active ad IDs, 4 concepts; none added or removed). The paid landing pages `/pm` and `/pm/main/v1` have the same copy as before. The only change is on the homepage: the promo bar now says "Recraft V4.1 Flash: The fastest model on the market". The ads don't link to the homepage, so this doesn't affect message match.
- **Why there's a PR today:** the three gaps (R1–R3) I found earlier today are still live on the pages, and none has an open PR. The GitHub API shows the repo has 0 open PRs, and it's still empty. The first run tried to open this PR but the token couldn't write. The second run skipped it. So the fix had never reached the repo, and this PR delivers it.
- **The biggest gap:** the **Upscale to 4K / print-ready** creative sends visitors to two pages, and neither one mentions upscaling, 4K or print.

## Where the ads actually land
Every Recraft creative links to a paid landing page under `/pm`, not to the bare homepage. I read the targets from each ad's `link_url` in the Ad Library:
- `https://recraft.ai/pm/?utm_source=facebook…` is the vector/SVG page.
- `https://www.recraft.ai/pm/main/v1?utm_source=facebook…` is the generic page.

So I judged message match against these two pages, which are the CTA pages the ads' visitors actually see. I've included the homepage structure below for reference.

## Live page structure (as of this run)
**/pm** (https://recraft.ai/pm/)
- **Hero:** "DROP A JPG. GET AN EDITABLE SVG." Sub: "Upload a logo, icon, lettering or illustration. Recraft vectorizes it in seconds and lets you edit every path and colour in the browser."
- **CTA:** "Start for free" in the header and hero, plus "Free to use. No credit card required. Works on any device."
- **Section order after the hero:**
  1. Logo strip "Loved by designers at"
  2. What you can make (tabs), with a CTA
  3. Consistent styles, with a CTA
  4. Testimonials: Playgama, an embroidery designer, a graphic designer. The vector quote sits here, well below the fold.
  5. Try it in Recraft, with a CTA
  6. Pricing table
  7. "Ready to start creating?" final CTA
- **Upscale/4K/print:** not mentioned anywhere on the page.
- **Mobile:** same order. Pricing rows collapse to "Plan details", and the testimonial carousel shows one card at a time.

**/pm/main/v1** (https://www.recraft.ai/pm/main/v1)
- **Hero:** a 3-slide carousel:
  1. "TASTEFULLY CRAFTED AI IMAGE MODELS"
  2. "VECTORS YOU CAN ACTUALLY EDIT"
  3. "A BRAND SET THAT HOLDS TOGETHER"
- **Section order after the hero:**
  1. Logo strip
  2. Five features: Prompt understanding, Aesthetic mastery, "UNMATCHED VECTOR GENERATION", Design assets, Consistent styles
  3. Articles
  4. Testimonials (proof)
  5. Try it in Recraft
  6. "Ready to start creating?"
- **CTA:** "Start for free" on every slide and section.
- **Mentions of the ad promises:** "icon", "upscale", "4K", "print", "JPG" and "SVG" appear **nowhere** on the page.
- **Mobile:** the header CTA shortens to "Start free". Otherwise the order is the same.

**Homepage** (https://www.recraft.ai/, reference only)
- **Promo bar:** "Recraft V4.1 Flash…" This is the one change since the last run.
- **Hero:** "TASTEFULLY CRAFTED AI IMAGE MODELS" with CTAs "Start creating" and "Get API". On mobile, "Get API" is hidden.
- **Section order after the hero:** logo strip → 5 features → testimonials → "Try in Recraft Studio / Try it free" → footer.
- **Upscaler, Vectorizer and Icons:** these only appear as footer links.

---

## Per creative

The Ad Library for Recraft AI (page id 361559813715585) shows about 23 results, which are 22 unique active ad IDs, all on FB and IG. Every ad uses the CTA button "Sign up" and the description "Free to start. No card needed."
Source: https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=ALL&view_all_page_id=361559813715585&search_type=page&media_type=all

### A. "Upscale any image to 4K" (8 ads, running for 2 days)
- **Links:**
  - https://www.facebook.com/ads/library/?id=1351920020096015 (goes to /pm)
  - also …?id=1630346431787876, 2088748265104581, 1746204436602270, 1792594955384511 (go to /pm)
  - also …?id=3108116902718135, 1125157440078039, 1430295042317990 (go to /pm/main/v1)
- **Copy:** body "Got a small image and need it print-ready? Upscale it to 4K in Recraft." Headline "Upscale any image to 4K". The visual is a large-format printer with the line "Too small to print? Upscale to 4K."
- **Promise:** a small or low-res image becomes a sharp 4K, print-ready file.
- **Audience:** people printing things, such as print-on-demand sellers, merch makers, and marketers with a small asset headed for print. They are not necessarily designers.
- **Does the page continue it? No.**
  - On /pm, the hero promises JPG→SVG vectorizing, which is a different job. Upscale, 4K and print don't appear anywhere on the page.
  - On /pm/main/v1, the promise also appears nowhere. The hero talks about "AI image models", vectors, and brand sets.
  - A visitor who clicked to fix a too-small image sees nothing that says this is the place to do it.
- **Fix: R1** (below).

### B. "Drop a JPG. Get an editable SVG." (12 ads, video and image, started today)
- **Links:**
  - https://www.facebook.com/ads/library/?id=2119007955355311 (goes to /pm; UGC video with a T-shirt logo)
  - also …?id=1062890446555843, 1804859447369608, 1418223223751289, 2540829573030844, 1615696030059456, 2563853590709812 (go to /pm)
  - also …?id=1614326270237557, 2056614111727374, 2544262482653138, 1530427782172956, 1707313861395818 (go to /pm/main/v1)
- **Copy:** body "Blurry logo? Turn any JPG or PNG into an editable SVG in seconds."
- **Promise:** a blurry raster logo becomes a clean, editable SVG in seconds.
- **Audience:** small-business owners, merch and T-shirt makers, and designers who have a bad logo file.
- **Does the page continue it?**
  - **/pm: yes, fully.** The hero headline repeats the ad word for word, and the sub names logo, icon and lettering. No change needed.
  - **/pm/main/v1: no.** The closest match is slide 2, "Vectors you can actually edit", which is abstract. It says nothing about JPG, PNG, SVG, logos or "blurry". Slide 1 is about image models in general. 5 of the 12 B ads land here.
- **Fix: R2** (below).

### C. "Create it in Recraft": illustrations, icons, logos and vectors from one prompt (1 ad, started today)
- **Link:** https://www.facebook.com/ads/library/?id=1592528655999168 (goes to /pm/main/v1). The visual is a flat basketball illustration.
- **Promise:** one prompt produces illustrations, icons, logos and vectors.
- **Audience:** marketers, founders and designers who need graphic assets quickly.
- **Does the page continue it? Partly.**
  - "Exceptional prompt understanding" and "Unmatched vector generation" point in the right direction.
  - But the page never names icons, logos or illustrations, and never ties them to "one prompt".
- **Fix: R3** (below; shared with D).

### D. "Can't find the icon? Create it." (1 ad, started today, low impressions)
- **Link:** https://www.facebook.com/ads/library/?id=911446388465811 (goes to /pm/main/v1). The visual is a prompt box reading "Planet wearing headphones".
- **Copy:** body "Can't find the right icon? Describe it and get it as an editable SVG." Description "Editable SVG. Sharp at any size."
- **Promise:** describe the icon you can't find and get it as an editable SVG.
- **Audience:** UI and web designers and developers who are searching icon libraries.
- **Does the page continue it? No.** The word "icon" never appears on /pm/main/v1.
- **Fix: R3** (below).

---

## Recommendations (3 max; all copy/section edits, none touch pricing, offers, checkout or quizzes)

### R1. Add an "Upscale to 4K" block where creative A lands
- **Gap:** Creative A ([1351920020096015](https://www.facebook.com/ads/library/?id=1351920020096015), [3108116902718135](https://www.facebook.com/ads/library/?id=3108116902718135)) promises "Upscale any image to 4K" and "print-ready". Neither /pm nor /pm/main/v1 mentions upscaling, 4K or print.
- **Why this continues the promise:** a print-focused visitor needs to see their exact problem named ("too small to print") and the exact outcome ("4K", "print-ready") right away. Otherwise they assume they landed on the wrong tool. The copy only uses claims Recraft makes on its own upscaler page: "up to 4K", "print-ready", and "Export at 300 DPI and CMYK" (https://www.recraft.ai/image-upscaler).
- **Exact change:**
  - **/pm/main/v1:** hero slide 2 becomes **"TOO SMALL TO PRINT? / UPSCALE IT TO 4K."** with the sub "Drop in a small image and get a sharp 4K version back in seconds. Headed to print? Export at 300 DPI and CMYK." The CTA stays "Start for free".
    - This slide replaces "A BRAND SET THAT HOLDS TOGETHER". That message is still covered by the "Consistent styles without training" feature further down.
  - **/pm:** a new section directly under the "Loved by designers at" logo strip, using the same headline and body, with CTA "Start for free".
    - The SVG hero stays, because it matches B, which sends the most traffic to /pm.
- **Supporting technique (not the reason for the change):**
  - Let's Enhance's upscaler ad ([4415145222069904](https://www.facebook.com/ads/library/?id=4415145222069904), "AI Image Upscaler: Enlarge Photos to 4K/8K+") lands on https://letsenhance.io/upscaler.
  - That page's hero repeats the number ("4K, 8K and beyond") and puts a "Print-ready: 300 DPI" proof point right in the hero.
  - It shows that repeating the ad's number and outcome word for word is how an upscaler page keeps the thread going.

### R2. Make the /pm/main/v1 lead slide the SVG promise
- **Gap:** Creative B ([1614326270237557](https://www.facebook.com/ads/library/?id=1614326270237557), [2119007955355311](https://www.facebook.com/ads/library/?id=2119007955355311)) promises "Blurry logo? Turn any JPG or PNG into an editable SVG". On /pm/main/v1, the first slide is "Tastefully crafted AI image models". The only vector slide is the abstract "Vectors you can actually edit", which never says JPG, PNG, SVG or logo.
- **Why this continues the promise:** B is the largest concept, with 5 of its ads landing on /pm/main/v1. Reusing the ad's headline as the first slide lets that visitor confirm straight away that they are in the right place. The "No file yet? Describe it" line also covers C and D visitors, who start from a prompt.
- **Exact change:** on /pm/main/v1, slide 1 becomes **"DROP A JPG. / GET AN EDITABLE SVG."** with the sub "Upload a blurry logo, icon or illustration and Recraft turns it into clean, editable vector paths in seconds. No file yet? Describe it and generate it as an SVG."
  - The old slide 1, "Tastefully crafted…", moves to slide 3.
  - "Vectors you can actually edit" is dropped because the new slide 1 replaces it.
- **Supporting technique:**
  - InstaSVG's ad ([1319389927061882](https://www.facebook.com/ads/library/?id=1319389927061882), "Turn Any Image into a Clean SVG") lands on a hero that repeats that line and names both ways in: "upload an image or describe what you want".
  - Recraft's own /pm already does this for B, and it matches fully.

### R3. Rename the vector feature so icons, logos and illustrations are named
- **Gap:**
  - Creative D ([911446388465811](https://www.facebook.com/ads/library/?id=911446388465811)) promises "Can't find the right icon? Describe it and get it as an editable SVG", but "icon" never appears on /pm/main/v1.
  - Creative C ([1592528655999168](https://www.facebook.com/ads/library/?id=1592528655999168)) promises "Illustrations, icons, logos and vectors, all from one prompt", but the page only says "Unmatched vector generation / Complex editable vector graphics".
- **Why this continues the promise:** icon-hunting designers and asset-hungry marketers scan for their own word, "icon" or "logo". Naming them, and echoing the ad's own "planet wearing headphones" example, closes the loop from the prompt box in the ad.
- **Exact change:** on /pm/main/v1, Feature 3 changes:
  - Headline: "UNMATCHED / VECTOR GENERATION" → **"ICONS, LOGOS & ILLUSTRATIONS / FROM ONE PROMPT"**
  - Caption: "Complex editable vector graphics" → **"Can't find the right icon? Describe it (say, "a planet wearing headphones") and get it back as an editable SVG, sharp at any size."**
- **Supporting technique:**
  - Kittl's Etsy ad ([2195237801372543](https://www.facebook.com/ads/library/?id=2195237801372543)) lands on kittl.com/get-started/etsy, whose hero names the audience's own job ("Sell more on Etsy…").
  - Runway's Aleph ad ([1332219041873617](https://www.facebook.com/ads/library/?id=1332219041873617)) lands on a page specific to that promise: runwayml.com/product/aleph-2.

## What I looked at but didn't recommend
- **Homepage (www.recraft.ai/):** it doesn't carry any of the four promises either, but no running creative sends traffic there. It's out of scope for message match today.
- **Separate landing pages per creative or UTM-driven heroes (like Zeely's /start/<promise>/ paths):** these would be the stronger long-term fix, but they are a routing or rebuild change, not a copy edit I can ship this week, so I didn't recommend them. I also didn't touch Zeely's quiz flow.
- **Other competitors:**
  - Canva's ads are generic and link to canva.com; its pages are blocked by Cloudflare.
  - Luma's ads all go to the generic lumalabs.ai/app.
  - Topaz's "until you zoomed in" ad ([1983047142622785](https://www.facebook.com/ads/library/?id=1983047142622785)) lands on a video page, which is itself a mismatch.
  - None of these gave usable technique evidence.
- **Pricing table on /pm:** a contract, so left untouched.

## Repo / PR notes
- The repo was empty (no commits and no branches). `main` has now been seeded with one commit: an **unmodified** transcription of the live copy (`recraft/{home,pm,pm-main-v1}/copy.md` and a README), so there is a base branch to open the PR against. None of the recommended changes are on `main`.
- All R1–R3 edits are only on `cta-scout/pm-message-match`: 2 files, `recraft/pm/copy.md` and `recraft/pm-main-v1/copy.md`.
- The PR has not been merged and I didn't call the merge endpoint. A human reviews and merges it.
