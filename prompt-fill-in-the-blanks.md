# Prompt A: rebuild Operation Luna Landing for a new area (fill in the blanks)

> **Use Claude Opus 5.5 Extra with Research Mode off, and turn on web search and code execution.** Claude does all the research itself in this chat, so the prompt spells out which sources to check for each building and when a neighborhood is finished. Without web search it can't price anything, and without code execution it can't resize the photo, build the share image, or test the page.


Fill in every [bracket] below, attach a photo, and paste the whole thing to Claude. The original page and its files are at https://github.com/bryancasler/operation-luna-landing (live at https://bryancasler.github.io/operation-luna-landing/); if Claude can't fetch GitHub in your session, download `index.html` and `operation-luna-landing-og.png` from that repo and attach them instead. Delete this paragraph before sending.

---

The starting point is a single-file web page called Operation Luna Landing. The source is at https://github.com/bryancasler/operation-luna-landing (everything is in `index.html`, with the share image `operation-luna-landing-og.png` beside it), and you can see it running at https://bryancasler.github.io/operation-luna-landing/. If you can't reach GitHub, I've attached the same two files. It was built to help one person find a studio near a specific park in Washington, DC with a large dog. I want you to rebuild it for a different search, keeping everything that makes it work and replacing everything that's specific to the old search. Read the whole file first so you understand how it's put together before you change anything.

## Who this is for

- I'm [YOUR NAME]. The page is for [WHO IT'S FOR AND HOW TO REFER TO EACH PERSON, OR "ME"]. Write it in my voice, in plain language, first person, warm but not gushing. Here are two or three messages I've actually written so you can match how I write: [PASTE 2 TO 3 SHORT MESSAGES OR TEXTS IN YOUR OWN VOICE].
- Unit type: [STUDIO / 1-BEDROOM / 2-BEDROOM]. Anything else about them that changes the search (work from home, a car, a schedule): [DETAILS].
- Dealbreakers: [ANYTHING THEY OR THE PETS NEED, AND ANY BUILDING RULE THAT RULES A PLACE OUT].

## Where and when

- The anchor is [ADDRESS OR CROSS STREETS, CITY, STATE]. Report walking time to it for every building and use it the way the old page used the park: the map rings, the walk filter, the card facts, and the walk times.
- Sweep these neighborhoods, one pass each: [NEIGHBORHOOD 1], [NEIGHBORHOOD 2], [NEIGHBORHOOD 3]. Cover the big management companies in this area plus smaller owner-managed buildings, and legitimate by-owner listings with a scam sanity check.
- Move-in window: [MONTH YEAR to MONTH YEAR]. Today's date is [DATE].

## Money

- Ceiling: [$X,XXX] a month with no discounts. Goal: [$X,XXX] or less. Keep the page's cost model: twelve months of rent minus advertised free months, plus pet rent, required building fees, one-time fees spread across the year, and the utilities they'd pay themselves, with a stated estimate for utilities when nothing is included. Show the no-deal number as the headline on each card. The old math charges pet rent once, for one dog, and leaves the one-time pet fee out because DC bans it. Pet rent is usually per pet, and one-time pet fees often are too, so count them for each pet unless the building says one charge covers all of them, and say which in each building's pet policy. Put non-refundable pet fees back into the one-time fees unless local law bars them; refundable deposits stay out, as before.

## Pets

- Pets: [KIND, HOW MANY, NAMES, AND SIZE AND BREED FOR ANY DOGS, OR "NONE"]. Re-point every dog-specific thing to these pets: does the building take them at all, how many, any size or breed limits, the deposit, the one-time fee, monthly pet rent, and rules specific to that kind of pet (declaw or indoor-only rules for cats, for example). Keep the "takes them in writing / not confirmed / sources disagree" pill logic. If there are no pets, take the pet pills, fees, and questions out rather than leaving them empty.
- The old page leans on a DC-only pet law (DC Law 25-308) that caps pet fees and voids weight limits. Replace that Good to know section with whatever actually governs pet fees, deposits, and pet rules where this search is, checked against primary sources: the statute or ordinance text itself, plus anything passed in the most recent legislative session that changed it. The DC law sat unenforced for over a year until a 2026 budget bill put it into effect, so don't trust a summary. If nothing caps the fees, say so plainly and use the advertised ones in the math. Remove every mention of the DC law from the cards, the questions, the pills, and the cost math unless the search is still in DC. With no pets, drop the section.

## What to keep from the old page

Keep the whole interface and behavior: the loading screen with the house, the opening note as a pop-up on first visit with the sparkle send-off and a "Read more" link afterward, the Good to know expanders, the sort options (score, cost, cost with discount, name), the schematic map with rings for walking minutes and numbered dots that follow the sort, the score-against-cost chart behind the Map toggle with clickable dots, the filters with single threshold sliders and the value bubble, the reset confirmations, the short list toggle and bottom-sheet with its own sort, the hide-a-building toggle with the poof animation, the per-building notes box, the review score that blends Google with ApartmentRatings and discounts small samples (explain the method in Good to know as the old page does), and the fact that everything the reader changes is saved in the browser. Don't remove features; re-point them.

Change what's specific: the title (something in the same spirit as "Operation Luna Landing"), the hook line, the opening note, the "Winter is when to sign" section (check whether the seasonal pattern holds for this market before keeping it), "Walk away if," "Already ruled out," the questions to ask every building, the building data, the map coordinates (place every building by its real direction and walking time from the anchor), and the footer's sources and date.

## Income-restricted units

The old page has an Inclusionary Zoning section that is DC-specific. Replace it with the local equivalent if one exists for these neighborhoods, with the real income limits and how the waitlist or lottery works, or drop the section if nothing applies. Don't leave DC program names anywhere on the page unless the search is in DC.

## Photo and share image

- I'm attaching a photo: [DESCRIBE IT IN ONE LINE]. Resize it to about 700 pixels on the long side, compress it to under 100 KB, and embed it as a data URI in the opening note with a caption in my voice, the way the old page embeds the dog photo. Remove the old dog photo entirely.
- Regenerate the share image (`operation-luna-landing-og.png`, 1200 by 630) with the new title, a one-line description, the new photo in the round frame, and the house. Rename it to match the new title, update the og:image, twitter:image, og:url, canonical, og:title, og:description, meta description, and the page title. Keep the house favicon.

## Publishing

I'll publish it on GitHub Pages at [https://USERNAME.github.io/REPO-NAME/]. Point every absolute URL in the head at that address. Deliver the same four files the old repo had: `index.html`, the share image PNG, `README.md` (rewritten for this search), and `.nojekyll`.

## How to work

Work straight through every neighborhood and the build without checking in. Stop and ask only when you can't go on without me: GitHub is unreachable, you need a fact only I know, a bracket above is still unfilled, or two readings of my instructions would produce different pages. If a reply runs out of room, end it with which neighborhoods are done and what's next, and pick up there when I say continue.

- Do the research neighborhood by neighborhood with these fields for every building: name, address, management, year built, unit and size, base rent, listing links, what utilities are included, monthly fees, current deals with conditions, one-time fees, air conditioning and heat type, in-unit laundry, walk time to the anchor and to transit, Google rating and count from the building's own profile, ApartmentRatings score and written-review count (say whether it's survey-based), recurring review themes, and the pet policy in full. Mark anything estimated versus verified, and date the data. The old page has no fields of its own for year built or walk time to transit (they show up only in free text, mostly the address, verdict, and air, heat, and laundry notes), so add both as data fields, name the station or stop for transit, and show both in each card's facts.
- Start each neighborhood by listing every candidate building before you research any of them. Search at least two listing sites (Apartments.com, Zillow, RentCafe, or Apartment List) and the big management companies' own sites, so the list doesn't depend on one site's coverage.
- For each building, check its own site (the pricing page and the pet policy, not just the home page), at least one listing site, its Google profile, and ApartmentRatings. ApartmentRatings often blocks automated reading; when it does, use what its pages show in search results and say so on the card. When two sources disagree on rent, fees, or the pet policy, record both and say which one the card uses.
- Keep a working notes file with the source and date for every rent, fee, and pet-policy figure, and write to it as you go. Fold each neighborhood into the page's data at the end of its pass, so nothing depends on search results from much earlier in the chat.
- A neighborhood is done when every candidate is either in the data or on the ruled-out list with a reason. Then re-check that the map has no overlapping labels, the filters' default values make sense for this price range (start tight enough that four to eight buildings show), and the score threshold default sits near the list average.
- Before you hand it back, run the same checks the old page went through: the HTML parses with no unclosed tags, the script has no errors in a headless browser, nothing overflows at 360, 390, and 1280 pixels wide, every dialog button works inside a sandboxed iframe (they must be click handlers, not form submits), a full reset returns the page to first-visit state, and the design detector flags nothing. Tell me what you verified and what you couldn't.
- Voice rules for anything I'll be reading or sending: no em dashes, no filler words, short sentences mixed with longer ones, define any local jargon the first time it appears, and say plainly when something is a guess.

When you're done, give me a short list of the buildings that cleared the filters, the one you'd call first and why, and anything I need to confirm by phone before they apply.
