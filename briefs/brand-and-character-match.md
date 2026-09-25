# Recraft CTA message-match brief (today's run)

**PR opened this run:** (this PR) (branch `cta-scout/brand-and-character-match`, not merged, waiting for human review)

## What changed since yesterday
- **The creative mix changed a lot.** Recraft launched two new concepts yesterday: **E, the "Bloom" brand campaign** and **F, "Generate perfect character"**. Together they make up **20 of the 24 active ads**. They link to both `/pm` and `/pm/main/v1`.
- **Ads that stopped** (checked on their Ad Library pages, which now say "Inactive"; they ran until yesterday):
  - All the "Upscale any image to 4K" ads that linked to `/pm`, e.g. [1351920020096015](https://www.facebook.com/ads/library/?id=1351920020096015), plus [3108116902718135](https://www.facebook.com/ads/library/?id=3108116902718135).
  - All the "Drop a JPG. Get an editable SVG." ads that linked to `/pm`, e.g. [2119007955355311](https://www.facebook.com/ads/library/?id=2119007955355311).
  - The one-prompt ad (C) and the icon ad (D) were already inactive yesterday.
- **Result for `/pm`:** no running ad sells what its hero says ("Drop a JPG. Get an editable SVG.").
- **The pages themselves have not changed.** The text of `recraft.ai/`, `/pm` and `/pm/main/v1` matches the earlier snapshot on desktop and mobile.
- **PR #1 is still not live.** It was merged earlier, but its copy (the upscale block, the SVG slide 1 and the icon feature) does not appear on the live pages. Either the deploy is still pending or the change didn't land.

## PR check (GitHub API, open and closed)
| PR | State | What it covers | Today |
|---|---|---|---|
| [#1](https://github.com/Kakoedlinnoeslovo/claude-cta-landing-pages/pull/1) | **MERGED** | Copy docs R1–R3: upscale block, SVG slide 1, icon feature | Already delivered, so not reopened. Not live yet. |
| [#2](https://github.com/Kakoedlinnoeslovo/claude-cta-landing-pages/pull/2) | OPEN | Built `/pm/main/v1` page: SVG hero, upscale, icon | Covers A and B, not E or F. It also **removes** the "A brand set that holds together" slide, which is the only line on `/pm/main/v1` that partly continues E. Reviewer should know this. |
| [#3](https://github.com/Kakoedlinnoeslovo/claude-cta-landing-pages/pull/3) | OPEN | Built `/pm` page with a two-card hero: SVG + upscale | Designed for A and B traffic to `/pm`, which has **stopped**. It does not cover E or F. |

No open or merged PR covers E or F, so I opened **one** new PR for them. It touches the same files as #2 and #3 (`pm/index.html`, `pm/main/v1/index.html`). Now that the ads have changed, it effectively replaces their hero sections, so the reviewer should pick one per route. I have not closed or merged anything.

## Live page structure (as of this run)
**`/pm`**
- Section order:
  1. Header "Start for free"
  2. Hero: **"DROP A JPG. GET AN EDITABLE SVG."**, with the sub "Upload a logo, icon, lettering or illustration…", the CTA "Start for free" and the microcopy "Free to use. No credit card required. Works on any device."
  3. Logo strip ("Loved by designers at")
  4. "What you can make" tabs: Vectors & typography / Photorealism / Design assets / Prompt understanding
  5. "Consistent styles without training"
  6. Testimonials: Ivan Korzun (Playgama), Vincent (embroidery), Sebastien T.
  7. "Try it in Recraft"
  8. **Pricing** (Free/Pro/Teams; a contract, not touched)
  9. Final CTA "Ready to start creating?"
- Proof sits below the fold, after the styles section.
- Mobile: same order; the pricing features collapse into "Plan details".

**`/pm/main/v1`**
- Section order:
  1. Header "Start for free" (mobile: "Start free")
  2. Hero carousel with three slides:
     - "TASTEFULLY CRAFTED AI IMAGE MODELS"
     - "VECTORS YOU CAN ACTUALLY EDIT"
     - "A BRAND SET THAT HOLDS TOGETHER"
  3. Logo strip
  4. Five features: prompt understanding, aesthetic mastery, vector generation, design assets, consistent styles
  5. Articles
  6. The same three testimonials
  7. "Try it in Recraft"
  8. Final CTA
- There is no pricing section.
- None of these words appear on either paid page: **brand campaign, product photos, launch, character, game**. Upscale/4K/print also don't appear.

**Homepage** (`recraft.ai/`): unchanged. The promo bar reads "Recraft V4.1 Flash" and the hero "Tastefully crafted AI image models". Paid ads don't link to it.

## Per creative
Active ads as of this run: 24 (Recraft's Meta page ID is 361559813715585). All run on Facebook and Instagram with the CTA "Sign up" and the link description "Free to start. No card needed."

### E: "Bloom" brand campaign (NEW, started yesterday; 10 ads)
- **Ads:**
  - Linking to `/pm`: [1525715616029644](https://www.facebook.com/ads/library/?id=1525715616029644) "From logo to launch.", [1756536708898900](https://www.facebook.com/ads/library/?id=1756536708898900) "She imagined it. She made it.", [1838633267310052](https://www.facebook.com/ads/library/?id=1838633267310052) "One idea. A whole brand.", [2190865681861820](https://www.facebook.com/ads/library/?id=2190865681861820) "Logo. Photos. Ready to launch.", [1861376208640041](https://www.facebook.com/ads/library/?id=1861376208640041) "Her vision. Made real."
  - Linking to `/pm/main/v1`: [1704747150628253](https://www.facebook.com/ads/library/?id=1704747150628253), [1421671353260483](https://www.facebook.com/ads/library/?id=1421671353260483), [1437206268331041](https://www.facebook.com/ads/library/?id=1437206268331041), [1640820400991631](https://www.facebook.com/ads/library/?id=1640820400991631), [947845541156772](https://www.facebook.com/ads/library/?id=947845541156772)
- **Creative:** a founder's face (UGC style) next to the "Bloom" nail-polish brand: logo, product shots and model photos. The overlay reads "She built her brand campaign in Recraft", with a "Try Recraft now" button. The body copy is "Create with Recraft. Free to start, no credit card required."
- **Promise:** one idea becomes a whole brand. You can take a logo all the way to launch-ready product photos and a campaign in one tool.
- **Implied audience:** founders and small-brand or DTC owners, especially beauty and consumer products. Most are not professional designers.
- **Does the page continue it?**
  - **`/pm`: No.** The hero talks about vectorizing a JPG, and the proof is all designers. "Consistent styles" is the closest idea, but it's abstract, comes third, and says nothing about a logo, product photos or a launch.
  - **`/pm/main/v1`: Weak.** Only carousel slide 3 ("A brand set that holds together") comes close, and most visitors never see slide 3.
- **Fix:** R7 (hero) and R8 (brand campaign section).

### F: "Generate perfect character" (NEW, started yesterday; 10 ads)
- **Ads:**
  - With the "Create with Recraft" body: [1789794925546225](https://www.facebook.com/ads/library/?id=1789794925546225) (`/pm`) and [28329625143366039](https://www.facebook.com/ads/library/?id=28329625143366039) (`/pm/main/v1`).
  - With the upscale body ("Got a small image and need it print-ready? Upscale it to 4K in Recraft."):
    - `/pm`: [1339087514756514](https://www.facebook.com/ads/library/?id=1339087514756514), [1110232068206894](https://www.facebook.com/ads/library/?id=1110232068206894), [1389788913141240](https://www.facebook.com/ads/library/?id=1389788913141240), [1602125834331437](https://www.facebook.com/ads/library/?id=1602125834331437)
    - `/pm/main/v1`: [1073753415639987](https://www.facebook.com/ads/library/?id=1073753415639987), [2102480330639721](https://www.facebook.com/ads/library/?id=2102480330639721), [1613375427116854](https://www.facebook.com/ads/library/?id=1613375427116854), [28474028432246514](https://www.facebook.com/ads/library/?id=28474028432246514)
- **Creative:** "GENERATE PERFECT CHARACTER" over a full-body game-hero character. The full prompt is printed on the ad (a young scavenger courier with a patched cloak and a mechanical arm). The same prompt appears in four styles: hand-painted, 32-bit pixel art, 3D toon and cel-shaded anime.
- **Promise:** describe a character once and get a polished, game-ready hero in the style you want.
- **Implied audience:** indie game developers, game artists and character designers.
- **Does the page continue it? No, on both routes.**
  - Neither page says "character" or "game".
  - The best proof, Playgama (a web-games company), sits unexplained in a generic testimonial carousel.
- **Fix:** R7 (hero) and R9 (character section).
- **Ad-side note (out of copy scope):** 8 of these ads pair the character image with **upscale** body copy, so the ad contradicts itself. I didn't make up a page fix for that. R9 only adds one truthful line so the upscale half isn't left out: "Need a small render bigger? Upscale it to 4K." The upscale claim comes from [recraft.ai/image-upscaler](https://www.recraft.ai/image-upscaler). The campaign owner should re-pair the body copy.

### A: "Upscale any image to 4K" (1 ad left)
- **Ad:** [1125157440078039](https://www.facebook.com/ads/library/?id=1125157440078039), linking to `/pm/main/v1`. The image shows a chat message ("Do you have this in higher resolution?"), then photo_small.jpg at 640×480, then a 4K straw bag, with "Upscale it in Recraft".
- **Promise:** turn a small image into a sharp 4K one that's ready to print.
- **Implied audience:** small sellers and marketers who've been asked for a higher-resolution file.
- **Does the page continue it?** Not on the live page. The fix is **already delivered** by merged PR #1 (upscale slide 2), and PR #2 has a built version. Nothing new is needed.
- **Status:** merged. The deploy is pending or didn't land.

### B: "Drop a JPG. Get an editable SVG." (3 ads left, video)
- **Ads:** [1614326270237557](https://www.facebook.com/ads/library/?id=1614326270237557), [2056614111727374](https://www.facebook.com/ads/library/?id=2056614111727374), [2544262482653138](https://www.facebook.com/ads/library/?id=2544262482653138), all linking to `/pm/main/v1`.
- **Promise:** blurry logo in, editable SVG out, in seconds.
- **Implied audience:** small-business owners and makers with a low-quality logo file.
- **Does the page continue it?** On the live `/pm/main/v1`, only through slide 2 ("Vectors you can actually edit"). The fix is **already delivered** by merged PR #1 (SVG slide 1).
- **Status:** merged, so nothing new is needed. The built `/pm/main/v1` page in the new PR keeps this copy directly under the hero.

## Recommendations (3; all are copy or section edits, no redesign; pricing, offer and checkout untouched)

### R7. Hero on `/pm` and `/pm/main/v1`: continue both new concepts in the first screen
- **Gap:**
  - E ([1525715616029644](https://www.facebook.com/ads/library/?id=1525715616029644), "From logo to launch.") and F ([1789794925546225](https://www.facebook.com/ads/library/?id=1789794925546225), "Generate perfect character") now make up **all** of `/pm`'s ad traffic and 10 of the 14 ads linking to `/pm/main/v1`.
  - Their visitors land on "Drop a JPG. Get an editable SVG." (`/pm`) or "Tastefully crafted AI image models" (`/pm/main/v1`). Neither continues either promise.
- **Why this continues the promise:**
  - The first thing each visitor reads repeats their own ad's headline.
  - Each card names its audience ("For founders & small brands" / "For game devs & artists"), so both groups can see they're in the right place without scrolling.
  - On mobile, the cards stack without thumbnails, so both fit in the first screen.
- **Exact change:**
  - Eyebrow "One idea is enough"
  - H1 **"Imagine it. Make it in Recraft."** This echoes E's "She imagined it. She made it."
  - Sub "Build a brand from logo to launch, or generate the perfect character from a single prompt."
  - Card 1: **"From logo to launch."** / "Your logo, product photos and campaign, made in one place and in one consistent style." / "Build your brand →"
  - Card 2: **"Generate the perfect character."** / "Describe your hero once, then get it hand-painted, in pixel art, as a 3D toon or in anime style." / "Create a character →"
  - CTA "Start for free" with "Free to use. No credit card required."
  - On `/pm/main/v1`, the SVG and upscale copy from merged PR #1 moves into two cards directly under the hero, so A and B keep their match.
- **Supporting technique (evidence only, not the reason for the change):**
  - Kittl ad [1125368037097786](https://www.facebook.com/ads/library/?id=1125368037097786) links to a page whose hero names the audience and the outcome ("All your small business content. Ready in a click."): get.kittl.com/smb-workflows.
  - Tripo ad [1966913807323436](https://www.facebook.com/ads/library/?id=1966913807323436) links to a game-development page (tripo3d.ai/lp/game-development).

### R8. "Logo. Photos. Ready to launch." section (replaces "Consistent styles without training")
- **Gap:**
  - E ads [2190865681861820](https://www.facebook.com/ads/library/?id=2190865681861820) ("Logo. Photos. Ready to launch.") and [1838633267310052](https://www.facebook.com/ads/library/?id=1838633267310052) ("One idea. A whole brand.") promise a path from logo to campaign.
  - The page only offers the abstract "Creating a custom style is as easy as dropping in your images."
- **Why this continues the promise:** it tells the capability the page already claims (styles) as the ad's own story: logo, then style and palette, then product photos and the campaign. That's written for a founder, not a designer, and uses the ad's own words.
- **Exact change:**
  - H2 **"Logo. Photos. Ready to launch."**
  - Body "One idea becomes a whole brand. Start with the mark, and everything after it looks like it came from the same hand."
  - Step 1: "**Design your logo.** Generate it as a real SVG with editable paths, sharp from a favicon to a banner."
  - Step 2: "**Turn it into your style.** Build a reusable style from your logo and lock your exact brand colours as a palette."
  - Step 3: "**Make the launch.** Generate product photos, mockups, social posts and ad creative that all look like the same brand."
  - CTA "Build your brand free"
  - Embedded @Recraftai video ["How to Use Recraft for beauty campaign design | Logos, Styles & Mockups"](https://www.youtube.com/watch?v=2gaPU65hg5g). It's a beauty brand, which matches Bloom.
- **Claims sourced from:** [From Logo to Full Brand Kit](https://www.recraft.ai/blog/from-logo-to-full-brand-kit) on Recraft's blog.
- **Supporting technique:** Kittl's small-business page repeats "launch assets that all look like the same brand" next to a CTA.

### R9. "Generate the perfect character." section (new)
- **Gap:** the F ads ([1789794925546225](https://www.facebook.com/ads/library/?id=1789794925546225), [1339087514756514](https://www.facebook.com/ads/library/?id=1339087514756514) and 8 more) show a prompt producing a hero character in four styles. Neither page mentions characters or games.
- **Why this continues the promise:**
  - The section repeats the ad's exact prompt and its four styles.
  - It adds what a game developer needs next: a reference sheet, so the character stays consistent.
  - It moves the Playgama quote here, where it works as game-industry proof.
- **Exact change:**
  - H2 **"Generate the perfect character."**
  - Prompt box: "Full-body game hero character: a young scavenger courier, patched layered cloak, mechanical left arm with glowing seams, heavy boots, satchel."
  - Style chips: Hand-painted / Pixel art / 3D toon / Cel-shaded anime
  - Step 1: "**Describe your hero once.** Same prompt, any style. Try eight directions at once in Exploration Mode."
  - Step 2: "**Get a reference sheet.** Front, profile, 3/4, back, expressions and colour swatches, so the character stays on-model."
  - Step 3: "**Ship it.** Covers, sprites, stickers and promo art. Need a small render bigger? Upscale it to 4K."
  - The Ivan Korzun (Playgama) quote, with a link to the case study
  - CTA "Create a character free"
  - Embedded @Recraftai video ["Recraft 3D tutorial: consistent 3D Styles, Characters & Icons"](https://www.youtube.com/watch?v=5EcTeB2c74Y)
- **Claims sourced from:**
  - [How to Build a Brand Mascot with AI](https://www.recraft.ai/blog/how-to-build-a-brand-mascot-with-ai) (Exploration Mode's 8 directions; the V4.1 reference sheet)
  - [Playgama case study](https://www.recraft.ai/blog/how-playgama-com-uses-recraft-to-power-global-game-launches)
  - [/image-upscaler](https://www.recraft.ai/image-upscaler) (up to 4K)
- **Supporting technique:** Tripo's game-development page labels its gallery "CHARACTERS, PROPS, ENVIRONMENTS", which names the asset the ad promised.

## What's in the PR
- `pm/index.html`: built `/pm` page in the house style (Geist font, #f6f6f7 background, #111 ink, black pill CTAs, "Start for free" / "Free to use. No credit card required.").
  - Implements R7–R9.
  - The live vector copy is kept, shorter, under "Also in Recraft".
  - Pricing appears only as an "unchanged" marker.
- `pm/main/v1/index.html`: built `/pm/main/v1` page. R7–R9, plus the A and B cards (from merged PR #1) under the hero.
- `recraft/pm/copy.md` and `recraft/pm-main-v1/copy.md`: the copy diff.
- `README.md`: adds a "Built pages" note.
- `briefs/brand-and-character-match.md`: this brief.
- Images come from recraft.ai/blog. Videos are youtube-nocookie embeds from @Recraftai, which loads the video only when clicked.

## Not recommended (out of scope or not supported by the evidence)
- **Re-pairing the upscale body copy on the 8 character ads.** This is an ad-side fix, not a page fix.
- **Routing each concept to its own URL.** That's an ads and routing decision.
- **No changes to pricing, offer terms or checkout.**
