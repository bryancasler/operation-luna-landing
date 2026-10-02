# Prompt B: rebuild Operation Luna Landing for a new area (Claude asks you one question at a time)

> **Use Claude Opus 5.5 Extra with Research Mode off, and turn on web search and code execution.** Claude does all the research itself in this chat, so the prompt spells out which sources to check for each building and when a neighborhood is finished. Without web search it can't price anything, and without code execution it can't resize the photo, build the share image, or test the page.


Paste everything below this line to Claude as your first message. You don't need to prepare anything; Claude asks for what it needs as it goes, including a photo.

---

I want you to rebuild a web page for a new apartment search, and I'd like you to interview me for the details before you start, one question at a time. Ask a single question, wait for my answer, then ask the next. Don't send me a list of questions to fill out. If an answer is vague, ask one follow-up. When you have everything, read the summary back to me for a yes before doing any work.

The starting point is a single-file web page called Operation Luna Landing. The source is at https://github.com/bryancasler/operation-luna-landing (everything is in `index.html`, with the share image `operation-luna-landing-og.png` beside it), and it's running at https://bryancasler.github.io/operation-luna-landing/. If you can't reach GitHub, tell me before the interview and I'll attach the two files. Read the whole file before you ask me anything, so your questions reflect what the page actually does.

It was built to help one person find a studio near a park in Washington, DC with a large dog. My search is different, and everything specific to the old one has to go, while everything that makes the page work stays. Don't assume anything about the new search that I haven't told you: who it's for, whether there are pets, and where it is all come from the interview.

## What to interview me about, in this order

1. Who the page is for, and whether I'm making it for them or for myself. Names, and how to refer to each person.
2. Pets: what kind, how many, their names, and size and breed for any dogs. There may be none.
3. The anchor: the address or cross streets the search centers on (a home, an office, a park), and why it matters.
4. The neighborhoods to sweep, one pass each. If I only name one, suggest the two or three next to it and ask which to include.
5. The unit type, and anything about the people that changes the search (a car, working from home, a schedule).
6. Move-in window, and today's date.
7. The monthly ceiling with no discounts, and the goal number.
8. Dealbreakers: anything the people or pets need (a ground floor, no carpet, a park nearby), and any building rule that would rule a place out.
9. Two or three short messages I've actually written to the people it's for, or anything I've written if it's for me, so you can match my voice.
10. A photo for the opening note (the pets, or the people if there are no pets), a one-line description, and the caption I'd put under it.
11. The GitHub Pages address I'll publish at, so every absolute URL in the head points there.
12. A working title for the page in the same spirit as "Operation Luna Landing," or tell me you'll propose three.

## What to keep from the old page

Keep the whole interface and behavior: the loading screen with the house, the opening note as a pop-up on first visit with the sparkle send-off and a "Read more" link afterward, the Good to know expanders, the sort options (score, cost, cost with discount, name), the schematic map with rings for walking minutes and numbered dots that follow the sort, the score-against-cost chart behind the Map toggle with clickable dots, the filters with single threshold sliders and the value bubble, the reset confirmations, the short list toggle and bottom sheet with its own sort, the hide-a-building toggle with the poof animation, the per-building notes box, the review score that blends Google with ApartmentRatings and discounts small samples (explain the method in Good to know as the old page does), and the fact that everything the reader changes is saved in the browser. Don't remove features; re-point them.

Change what's specific: the title, the hook line, the opening note (in my voice: plain language, first person, warm but not gushing), the "Winter is when to sign" section (check whether the seasonal pattern holds in this market before keeping it), "Walk away if," "Already ruled out," the questions to ask every building, the building data, the map coordinates, and the footer's sources and date. The anchor replaces the park everywhere: the map rings, the walk filter, the card facts, and the walk times. Place every building by its real direction and walking time from it.

Re-point every dog-specific thing to the pets I describe: does the building take them at all, how many, any size or breed limits, the deposit, the one-time fee, monthly pet rent, and rules specific to that kind of pet (declaw or indoor-only rules for cats, for example). Keep the "takes them in writing / not confirmed / sources disagree" pill logic. If there are no pets, take the pet pills, fees, and questions out rather than leaving them empty.

Keep the cost model: twelve months of rent minus advertised free months, plus pet rent, required building fees, one-time fees spread across the year, and the utilities they'd pay themselves, with a stated estimate when nothing is included; the no-deal number stays the headline on each card. The old math charges pet rent once, for one dog, and leaves the one-time pet fee out because DC bans it. Pet rent is usually per pet, and one-time pet fees often are too, so count them for each pet unless the building says one charge covers all of them, and say which in each building's pet policy. Put non-refundable pet fees back into the one-time fees unless local law bars them; refundable deposits stay out, as before.

## Local rules

- The old page's pet law section (DC Law 25-308) caps pet fees and voids weight limits, but only in DC. Replace it with whatever actually governs pet fees, deposits, and pet rules where the new search is, checked against primary sources: the statute or ordinance text itself, plus anything passed in the most recent legislative session that changed it. The DC law sat unenforced for over a year until a 2026 budget bill put it into effect, so don't trust a summary. If nothing caps the fees, say so and use the advertised ones. Remove every mention of the DC law from the cards, the questions, the pills, and the cost math unless the search is still in DC. With no pets, drop the section.
- The old page's Inclusionary Zoning section is DC-specific. Replace it with the local equivalent if one exists for the new neighborhoods, with real income limits and how the waitlist or lottery works, or drop it. No DC program names unless the search is in DC.

## Photo and share image

Resize the photo to about 700 pixels on the long side, compress it to under 100 KB, and embed it as a data URI in the opening note with my caption, the way the old page embeds the dog photo. Remove the old dog photo entirely. Regenerate the share image (1200 by 630) with the new title, a one-line description, the new photo in the round frame, and the house. Rename it to match the new title and update og:image, twitter:image, og:url, canonical, og:title, og:description, the meta description, and the page title. Keep the house favicon.

## How to work once the interview is done

Once I've said yes to the summary, work straight through every neighborhood and the build without checking in. Stop and ask only when you can't go on without me: GitHub is unreachable, you need a fact only I know, or two readings of my instructions would produce different pages. If a reply runs out of room, end it with which neighborhoods are done and what's next, and pick up there when I say continue.

- Research neighborhood by neighborhood with these fields for every building: name, address, management, year built, unit and size, base rent, listing links, what utilities are included, monthly fees, current deals with conditions, one-time fees, air conditioning and heat type, in-unit laundry, walk time to the anchor and to transit, Google rating and count from the building's own profile, ApartmentRatings score and written-review count (say whether it's survey-based), recurring review themes, and the pet policy in full. Mark estimated versus verified, and date the data. The old page has no fields of its own for year built or walk time to transit (they show up only in free text, mostly the address, verdict, and air, heat, and laundry notes), so add both as data fields, name the station or stop for transit, and show both in each card's facts.
- Start each neighborhood by listing every candidate building before you research any of them. Search at least two listing sites (Apartments.com, Zillow, RentCafe, or Apartment List) and the big management companies' own sites, so the list doesn't depend on one site's coverage.
- For each building, check its own site (the pricing page and the pet policy, not just the home page), at least one listing site, its Google profile, and ApartmentRatings. ApartmentRatings often blocks automated reading; when it does, use what its pages show in search results and say so on the card. When two sources disagree on rent, fees, or the pet policy, record both and say which one the card uses.
- Keep a working notes file with the source and date for every rent, fee, and pet-policy figure, and write to it as you go. Fold each neighborhood into the page's data at the end of its pass, so nothing depends on search results from much earlier in the chat.
- A neighborhood is done when every candidate is either in the data or on the ruled-out list with a reason. Then re-check that the map has no overlapping labels, the filters' defaults make sense for this price range (tight enough that four to eight buildings show), and the score threshold default sits near the list average.
- Before you hand it back, run the checks the old page went through: the HTML parses with no unclosed tags, the script has no errors in a headless browser, nothing overflows at 360, 390, and 1280 pixels wide, every dialog button works inside a sandboxed iframe (click handlers, not form submits), a full reset returns the page to first-visit state, and the design detector flags nothing. Tell me what you verified and what you couldn't.
- Deliver the same four files the old repo had: `index.html`, the share image PNG, `README.md` rewritten for this search, and `.nojekyll`.
- Voice rules for anything I'll be reading or sending: no em dashes, no filler words, short sentences mixed with longer ones, define local jargon the first time it appears, and say plainly when something is a guess.

When you're done, give me a short list of the buildings that cleared the filters, the one you'd call first and why, and anything I need to confirm by phone before they apply.

Start the interview with question 1.
