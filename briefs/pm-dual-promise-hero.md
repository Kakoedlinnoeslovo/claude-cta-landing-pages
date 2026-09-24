# Recraft CTA message-match brief (cta-scout, today's run)

**PR opened this run:** PR_URL_PLACEHOLDER (branch `cta-scout/pm-dual-promise-hero`, **not merged**. A human needs to review and merge it.)
**Deliverable in the PR:** `pm/index.html`, a built, self-contained page for **https://recraft.ai/pm/**, the route that 9 of today's 14 active ad IDs link to. It uses the house style from `templates/pm-improved-reference.html`, real recraft.ai/blog images and two youtube-nocookie embeds from @Recraftai. `recraft/pm/copy.md` is updated to match the page.

## What changed since the last run
- **Creatives:** yesterday there were 22 active ad IDs across 4 concepts. As of this run there are **14 active IDs across 2 concepts**. Concept C ("Create it in Recraft", [1592528655999168](https://www.facebook.com/ads/library/?id=1592528655999168)) and concept D ("Can't find the icon? Create it.", [911446388465811](https://www.facebook.com/ads/library/?id=911446388465811)) are now **Inactive**. Each ran for about 12 hours yesterday. Six more A/B IDs also dropped out. The ads still running are the **Upscale-4K** ads (A) and the **JPG→SVG** ads (B).
- **Where the traffic goes now:** on **/pm**, 5 active IDs are Upscale ads and 4 are SVG ads, so **Upscale ads are the majority of /pm traffic**. On /pm/main/v1 there are 2 Upscale IDs and 3 SVG IDs.
- **Live pages:** home, /pm and /pm/main/v1 are word-for-word the same as last run on both desktop and mobile. There are still 0 mentions of upscale, 4K or print on /pm or /pm/main/v1.
- **Repo:** I checked through the GitHub API (all PR states):
  - **PR #1**, [cta-scout/pm-message-match](https://github.com/Kakoedlinnoeslovo/claude-cta-landing-pages/pull/1): **MERGED**. It delivered R1–R3 as copy docs (an upscale section under the /pm logo strip, plus the SVG slide, upscale slide and icon feature on /pm/main/v1). That copy is still **not on the live pages**, so either the deploy is pending or it didn't land. I did **not** reopen it.
  - **PR #2**, [cta-scout/pm-designed-page](https://github.com/Kakoedlinnoeslovo/claude-cta-landing-pages/pull/2): **OPEN**. It's a built page for **/pm/main/v1** (R1–R3). I opened no duplicate and didn't touch /pm/main/v1 in the new PR.
  - **Gap not covered by either PR:** no PR builds **/pm**, and no PR puts the Upscale promise in /pm's **first screen**. PR #1 placed it *below the logo strip*, under an SVG-only hero. That is the new PR.

## Live page snapshot (as of this run)
- **/pm** (desktop): header "Start for free" → hero **"DROP A JPG. GET AN EDITABLE SVG."** with sub "Upload a logo, icon, lettering or illustration…" → CTA "Start for free" plus "Free to use. No credit card required. Works on any device." → "Loved by designers at" logos → What you can make (tabs) → Consistent styles → testimonials (Korzun, Vincent, Sebastien T.) → Try it in Recraft → pricing table (a contract, left untouched) → "Ready to start creating?" final CTA. Proof (logos) sits under the hero. **Mobile:** same order, and the first screen shows only the SVG hero.
- **/pm/main/v1**: a 3-slide hero carousel ("Tastefully crafted AI image models" / "Vectors you can actually edit" / "A brand set that holds together") → logos → 5 features → Articles → testimonials → Try it → "Ready to start creating?". The mobile header CTA reads "Start free".
- **Home**: promo bar "Recraft V4.1 Flash" → "Tastefully crafted AI image models" hero with "Start creating" / "Get API" buttons → logos → features → testimonials → footer. No ad links here.

---

## Per creative

### A: "Upscale any image to 4K" (active since 3 days ago; 7 active IDs)
- **Links:** [1351920020096015](https://www.facebook.com/ads/library/?id=1351920020096015), [1630346431787876](https://www.facebook.com/ads/library/?id=1630346431787876), [2088748265104581](https://www.facebook.com/ads/library/?id=2088748265104581), [1746204436602270](https://www.facebook.com/ads/library/?id=1746204436602270), [1792594955384511](https://www.facebook.com/ads/library/?id=1792594955384511) → **/pm**; [3108116902718135](https://www.facebook.com/ads/library/?id=3108116902718135), [1125157440078039](https://www.facebook.com/ads/library/?id=1125157440078039) → /pm/main/v1.
- **Promise:** "Got a small image and need it print-ready? Upscale it to 4K in Recraft." The headline is "Upscale any image to 4K" and the description is "Free to start. No card needed." The visual is a large-format printer with the line "Too small to print? Upscale to 4K."
- **Implied audience:** people with a low-res image that has to go to print, such as print-on-demand sellers, small-business owners and marketers. They are not designers looking for a vector tool.
- **Does /pm continue it?** **No.** The live /pm says nothing about upscale, 4K or print. After merged PR #1 ships, the promise will appear only *below the logo strip*, under an SVG hero that talks about "logo, icon, lettering". On mobile that is below the first screen. Most /pm ad traffic now comes from this concept, yet its visitors first read about a different job.
- **Fix:** R4 and R5 below.

### B: "Drop a JPG. Get an editable SVG." (active since yesterday; 7 active IDs; video + image)
- **Links:** [2119007955355311](https://www.facebook.com/ads/library/?id=2119007955355311) (video), [1062890446555843](https://www.facebook.com/ads/library/?id=1062890446555843), [1804859447369608](https://www.facebook.com/ads/library/?id=1804859447369608), [2563853590709812](https://www.facebook.com/ads/library/?id=2563853590709812) → **/pm**; [1614326270237557](https://www.facebook.com/ads/library/?id=1614326270237557), [2056614111727374](https://www.facebook.com/ads/library/?id=2056614111727374), [2544262482653138](https://www.facebook.com/ads/library/?id=2544262482653138) → /pm/main/v1.
- **Promise:** "Blurry logo? Turn any JPG or PNG into an editable SVG in seconds." The headline is "Drop a JPG. Get an editable SVG." The video is a UGC creator vectorizing a T-shirt logo on camera.
- **Implied audience:** small-brand owners, merch and T-shirt makers and designers who have a blurry raster logo and need a clean vector.
- **Does /pm continue it?** **In copy, yes.** The hero headline is the ad headline word for word. **Proof is the weak spot:** the video ad *shows* the conversion happening "in seconds", but /pm shows no conversion at all, only static generation tabs.
- **Does /pm/main/v1 continue it?** Not live today. It's covered by merged PR #1 (copy) and open PR #2 (built page), so no new action.
- **Fix:** R4 keeps the headline exactly, so the match isn't lost. R6 below adds the demo.

### C: "Create it in Recraft" and D: "Can't find the icon? Create it."
- **Now inactive** ([1592528655999168](https://www.facebook.com/ads/library/?id=1592528655999168), [911446388465811](https://www.facebook.com/ads/library/?id=911446388465811)). I've dropped them from this run's gap analysis. **Note for PR #2's reviewer:** its "Icons, logos & illustrations from one prompt" section (R3) served these two creatives, which have stopped. It does no harm, but it no longer serves a running ad. Consider moving it below the upscale section or trimming it.

---

## Recommendations (3, all on /pm; built in `pm/index.html`)

### R4: Dual-promise hero, so both /pm ad audiences see their own promise first
- **Observed gap:** Upscale ad [1351920020096015](https://www.facebook.com/ads/library/?id=1351920020096015) and 4 sibling IDs promise "Upscale it to 4K… print-ready" and send visitors to /pm. The /pm hero offers only "Drop a JPG. Get an editable SVG." and "logo, icon, lettering or illustration". SVG ad [2119007955355311](https://www.facebook.com/ads/library/?id=2119007955355311) and 3 sibling IDs land on the same hero and *do* match it. One hero serves two different promises, and the majority audience gets the wrong one.
- **Why this continues the promise:** each audience finds its ad's own question and headline in the first screen. "Too small to print?" + "Upscale any image to 4K." is the ad's exact words. "Blurry logo?" + "Drop a JPG. Get an editable SVG." is also verbatim, so the SVG ads keep their full match. On mobile, the cards are compacted so that both headlines and both CTAs sit in the first screen.
- **Exact change** (replaces the current /pm hero; the rest of the page order stays the same):
  - Eyebrow: **"Fix the file you already have"**. Desktop-only intro: "Two jobs, one free Recraft account. Pick the one you came for."
  - Card 1: kicker **"Blurry logo?"**, headline **"DROP A JPG. / GET AN EDITABLE SVG."**, and the current sub unchanged. Chips "JPG, PNG, WebP in · SVG out · Every path editable". CTA **"Start for free"**, link "Watch it vectorize".
  - Card 2: kicker **"Too small to print?"**, headline **"UPSCALE ANY IMAGE / TO 4K."**, sub "Drop in a small image and get a sharp 4K version back in seconds. Headed to print? Export at 300 DPI and CMYK." Chips "Up to 4K · 300 DPI · CMYK". CTA **"Start for free"**, link "See before & after".
  - Under both cards: "Free to use. No credit card required. Works on any device."
  - Claims source: Recraft's own [/image-upscaler](https://www.recraft.ai/image-upscaler) page ("up to 4K", "print-ready", "300 DPI and CMYK") and [/ai-image-vectorizer](https://www.recraft.ai/ai-image-vectorizer) page ("PNG, JPG or WebP to SVG… in seconds").
- **Supporting technique (not the reason for the change):** Let's Enhance's upscale ad [4415145222069904](https://www.facebook.com/ads/library/?id=4415145222069904) lands on [letsenhance.io/upscaler](https://letsenhance.io/upscaler). Its hero repeats the ad's number ("4K, 8K and beyond") and shows proof chips, one of which is "Print-ready: Reach 300 DPI". Playground AI's vectorize ad [2306552059903070](https://www.facebook.com/ads/library/?id=2306552059903070) lands on [playgroundai.com/cricut](https://playgroundai.com/cricut), where the hero names the exact output ("export a layered SVG"). Kittl's home page puts intent chips under the hero so each visitor can pick their job.

### R5: Prove the upscale promise right under the hero, not just state it
- **Observed gap:** Ad [1351920020096015](https://www.facebook.com/ads/library/?id=1351920020096015) sells an *outcome*: a small image becomes something print-ready (the creative shows a printer). Even with merged PR #1, /pm only *states* the claim. It shows no before/after, no steps, and doesn't show the job being done.
- **Why this continues the promise:** someone with an image that's too small wants to see small → large → print before signing up. The section shows exactly that, using only Recraft's own material.
- **Exact change** (this is the section PR #1 placed directly under the logo strip; PR #1's headline and body are kept word for word):
  - Keep "TOO SMALL TO PRINT? / UPSCALE IT TO 4K." and "Drop in a small image… Export at 300 DPI and CMYK."
  - **Add 3 steps** (from /image-upscaler): "Upload an image. Drag and drop a JPG, PNG or WebP." · "Click Upscale. Resolution goes up to 4K while the detail stays sharp." · "Export and use. Download as PNG, JPG, TIFF or PDF, at 300 DPI and CMYK for print."
  - **Add a video:** @Recraftai "How to upscale an image with Recraft" (youtube-nocookie `4lx2_7mz0Tk`).
  - The hero card uses the small→large food-truck image from Recraft's blog post [AI Upscaling](https://www.recraft.ai/blog/ai-upscaling-photos-how-to-transform-images-with-high-quality-enhancement).
  - Add a source line linking [/image-upscaler](https://www.recraft.ai/image-upscaler) and [/features/dpi](https://www.recraft.ai/features/dpi).
- **Supporting technique:** Let's Enhance ([/upscaler](https://letsenhance.io/upscaler)) puts a before/after slider directly under its hero, followed by a "How to upscale" section in 3 steps.

### R6: Show the JPG→SVG conversion in motion, as the video ad does
- **Observed gap:** Video creative [2119007955355311](https://www.facebook.com/ads/library/?id=2119007955355311) shows a creator turning a blurry logo into an SVG on camera. /pm continues the words but not the demo, so "in seconds" is never shown.
- **Why this continues the promise:** people who clicked a demo video expect to see the same demo on the page. Showing the vectorize flow keeps the ad's format and its "in seconds" claim going.
- **Exact change** (new section after R5):
  - Headline: "WATCH A JPG BECOME / AN EDITABLE SVG."
  - Body: "Blurry logo? Upload it and Recraft turns it into clean vector paths in seconds. Recolour it, simplify it, then export a file that stays sharp at any size."
  - 3 steps (from /ai-image-vectorizer): Upload · Click Vectorize · Edit and download.
  - Video: @Recraftai "Convert Any Image to Vector in Seconds with Recraft" (youtube-nocookie `k-rzbQvduzo`). The hero card image is the vector-paths illustration from Recraft's blog post [Best Image Vectorizers](https://www.recraft.ai/blog/best-image-vectorizers).
- **Supporting technique:** InstaSVG's ad [1319389927061882](https://www.facebook.com/ads/library/?id=1319389927061882) ("Turn Any Image into a Clean SVG") lands on instasvg.com, which repeats the headline and walks through upload → style → download.

**Left untouched on purpose:** the pricing table (Free/Pro/Teams, a contract; it's shown only as an "unchanged" marker), offer terms, checkout and signup flow. All CTAs stay "Start for free" with "Free to use. No credit card required." Testimonials, Consistent styles, Try it in Recraft and the final CTA keep their live copy exactly.

## Not reopened / watch list
- **PR #1 (merged):** R1–R3 copy is delivered but not yet live on /pm or /pm/main/v1. Either the deploy is pending or the change didn't land. Please check the Framer publish.
- **PR #2 (open):** built /pm/main/v1 page. The dual-promise idea from R4 could also help its hero, since 2 Upscale IDs land there. That's a note for PR #2's reviewer, not a new PR.
- Routing Upscale ads to a dedicated upscale page is an ad-side change and outside copy scope. R4 is the copy-side fix.
