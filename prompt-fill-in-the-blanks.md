# Prompt A: rebuild Operation Luna Landing for a new area (fill in the blanks)

> **Use Claude Fable 5.1 Max with Research Mode enabled.** This rebuild depends on several long research passes and a lot of code work in one session. A smaller model or a session without Research Mode will cut corners on the building data.


Fill in every [bracket] below, attach a photo, and paste the whole thing to Claude. The original page and its files are at https://github.com/bryancasler/operation-luna-landing (live at https://bryancasler.github.io/operation-luna-landing/); if Claude can't fetch GitHub in your session, download `index.html` and `operation-luna-landing-og.png` from that repo and attach them instead. Delete this paragraph before sending.

---

The starting point is a single-file web page called Operation Luna Landing. The source is at https://github.com/bryancasler/operation-luna-landing (everything is in `index.html`, with the share image `operation-luna-landing-og.png` beside it), and you can see it running at https://bryancasler.github.io/operation-luna-landing/. If you can't reach GitHub, I've attached the same two files. It was built to help one person find a studio near a specific park in Washington, DC with a large dog. I want you to rebuild it for a different search, different people, and a different city, keeping everything that makes it work and replacing everything that's specific to the old search. Read the whole file first so you understand how it's put together before you change anything.

## Who this is for

- I'm [YOUR NAME]. I'm building this for my brother, [BROTHER'S NAME], and his wife, [WIFE'S NAME]. They have two cats: [CAT 1 NAME] and [CAT 2 NAME]. Write the page as me writing to them, in plain language, first person, warm but not gushing. Here are two or three messages I've actually sent them so you can match how I write: [PASTE 2 TO 3 SHORT MESSAGES OR TEXTS IN YOUR OWN VOICE].
- Household: [2 adults, 2 cats]. Unit type: [1-bedroom / 2-bedroom / studio also fine?]. Anything else about them that changes the search (work from home, a car, a schedule): [DETAILS].

## Where and when

- The anchor is my home at [YOUR ADDRESS OR CROSS STREETS, CITY, VA]. The whole point is walking distance from me: report walking time to that address for every building and use it the way the old page used the park (the map rings, the walk filter, the card facts).
- Sweep these neighborhoods, one research pass each, comprehensively: [NEIGHBORHOOD 1], [NEIGHBORHOOD 2], [NEIGHBORHOOD 3]. Cover the big management companies in this area plus smaller owner-managed buildings, and legitimate by-owner listings with a scam sanity check.
- Move-in window: [MONTH YEAR to MONTH YEAR]. Today's date is [DATE].

## Money

- Ceiling: [$X,XXX] a month with no discounts. Goal: [$X,XXX] or less. Keep the page's cost model: twelve months of rent minus advertised free months, plus pet rent, required building fees, one-time fees spread across the year, and the utilities they'd pay themselves, with a stated estimate for utilities when nothing is included. Show the no-deal number as the headline on each card.

## Pets

- This search is for two cats, not a dog. Replace every dog-specific thing with the cat equivalent: does the building take cats at all, how many pets, cat deposit, one-time cat fee, monthly cat rent, and any declaw or indoor-only rules. Keep the "takes them in writing / not confirmed / sources disagree" pill logic.
- The old page leans on a DC-only pet law (DC Law 25-308) that caps pet fees and voids weight limits. That does not apply in Virginia. Remove that Good to know section and every mention of it in the cards, the questions, the pills, and the cost math, and replace it with whatever actually governs pet fees and deposits in Virginia right now, checked against primary sources. If nothing caps them, say so plainly and use the advertised fees in the math.

## What to keep from the old page

Keep the whole interface and behavior: the loading screen with the house, the opening note as a pop-up on first visit with the sparkle send-off and a "Read more" link afterward, the Good to know expanders, the sort options (score, cost, cost with discount, name), the schematic map with rings for walking minutes and numbered dots that follow the sort, the score-against-cost chart behind the Map toggle with clickable dots, the filters with single threshold sliders and the value bubble, the reset confirmations, the short list toggle and bottom-sheet with its own sort, the hide-a-building toggle with the poof animation, the per-building notes box, the review score that blends Google with ApartmentRatings and discounts small samples (explain the method in Good to know as the old page does), and the fact that everything the reader changes is saved in the browser. Don't remove features; re-point them.

Change what's specific: the title (something in the same spirit, using [CAT 1 NAME] or both cats), the hook line, the opening note, the "Winter is when to sign" section (check whether the seasonal pattern holds for this market before keeping it), "Walk away if," "Already ruled out," the questions to ask every building, the building data, the map coordinates (place every building by its real direction and walking time from my address), and the footer's sources and date.

## Income-restricted units

The old page has an Inclusionary Zoning section that is DC-specific. Replace it with the local equivalent if one exists for these neighborhoods (for example, Arlington's and Alexandria's affordable dwelling unit programs), with the real income limits and how the waitlist or lottery works, or drop the section if nothing applies. Don't leave DC program names anywhere on the page.

## Photo and share image

- I'm attaching a photo of the cats: [DESCRIBE IT, e.g., "both cats on the windowsill"]. Resize it to about 700 pixels on the long side, compress it to under 100 KB, and embed it as a data URI in the opening note with a caption in my voice, the way the old page embeds the dog photo. Remove the old dog photo entirely.
- Regenerate the share image (`operation-luna-landing-og.png`, 1200 by 630) with the new title, a one-line description, the cat photo in the round frame, and the house. Rename it to match the new title, update the og:image, twitter:image, og:url, canonical, og:title, og:description, meta description, and the page title. Keep the house favicon.

## Publishing

I'll publish it on GitHub Pages at [https://USERNAME.github.io/REPO-NAME/]. Point every absolute URL in the head at that address. Deliver the same four files the old repo had: `index.html`, the share image PNG, `README.md` (rewritten for this search), and `.nojekyll`.

## How to work

- Do the research neighborhood by neighborhood with the same fields the old page uses for every building: name, address, management, year built, unit and size, base rent, listing links, what utilities are included, monthly fees, current deals with conditions, one-time fees, air conditioning and heat type, in-unit laundry, walk time to my address and to transit, Google rating and count from the building's own profile, ApartmentRatings score and written-review count (say whether it's survey-based), recurring review themes, and the cat policy in full. Mark anything estimated versus verified, and date the data.
- After each pass, fold the buildings into the page's data, keep a ruled-out list with reasons, and re-check that the map has no overlapping labels, the filters' default values make sense for this price range (start tight enough that four to eight buildings show), and the score threshold default sits near the list average.
- Before you hand it back, run the same checks the old page went through: the HTML parses with no unclosed tags, the script has no errors in a headless browser, nothing overflows at 360, 390, and 1280 pixels wide, every dialog button works inside a sandboxed iframe (they must be click handlers, not form submits), a full reset returns the page to first-visit state, and the design detector flags nothing. Tell me what you verified and what you couldn't.
- Voice rules for anything I'll be reading or sending: no em dashes, no filler words, short sentences mixed with longer ones, define any local jargon the first time it appears, and say plainly when something is a guess.

When you're done, give me a short list of the buildings that cleared the filters, the one you'd call first and why, and anything I need to confirm by phone before they apply.
