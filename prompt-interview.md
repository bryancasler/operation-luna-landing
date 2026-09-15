# Prompt B: rebuild Operation Luna Landing for a new area (Claude asks you one question at a time)

> **Use Claude Fable 5.1 Max with Research Mode enabled.** This rebuild depends on several long research passes and a lot of code work in one session. A smaller model or a session without Research Mode will cut corners on the building data.


Paste everything below this line to Claude as your first message. You don't need to prepare anything except a photo of the cats; Claude will ask for it when it's time. Delete this paragraph before sending.

---

I want you to rebuild a web page for a new apartment search, and I'd like you to interview me for the details before you start, one question at a time. Ask a single question, wait for my answer, then ask the next. Don't send me a list of questions to fill out. If an answer is vague, ask one follow-up. When you have everything, read the summary back to me for a yes before doing any work.

The starting point is a single-file web page called Operation Luna Landing. The source is at https://github.com/bryancasler/operation-luna-landing (everything is in `index.html`, with the share image `operation-luna-landing-og.png` beside it), and it's running at https://bryancasler.github.io/operation-luna-landing/. If you can't reach GitHub, tell me before the interview and I'll attach the two files. Read the whole file before you ask me anything, so your questions reflect what the page actually does.

It was built to help one person find a studio near a park in Washington, DC with a large dog. My search is different, and everything specific to the old one has to go, while everything that makes the page work stays. Here is what I know already, so don't ask about these:

- It's for my brother and his wife and their two cats, and I'm making it for them. The page should read as me writing to them: plain language, first person, warm but not gushing.
- The anchor is my home in Virginia, and the point is walking distance from me. My address replaces the park in everything: the map rings, the walk filter, the card facts, the walk times.
- The old page's DC pet law section (DC Law 25-308) does not apply in Virginia. Remove it and every mention of it from the cards, the questions, the pills, and the cost math, and replace it with whatever actually governs pet fees and deposits in Virginia right now, checked against primary sources. If nothing caps them, say so and use the advertised fees.
- The old page's Inclusionary Zoning section is DC-specific. Replace it with the local equivalent if one exists for my neighborhoods (Arlington's and Alexandria's affordable dwelling unit programs, for example), with real income limits and how the waitlist works, or drop it. No DC program names anywhere.

## What to interview me about, in this order

1. My name and how to refer to my brother, his wife, and each cat.
2. My address or cross streets, so the map and walk times have their center.
3. The neighborhoods to sweep, one research pass each. If I only name one, suggest the two or three next to it and ask which to include.
4. The unit type they want, and anything about them that changes the search (a car, working from home, a schedule).
5. Move-in window, and today's date.
6. The monthly ceiling with no discounts, and the goal number.
7. Cat specifics: anything the cats need (ground floor, no carpet, a window), and any building rule that would rule a place out for them.
8. Two or three short messages I've actually sent my brother, so you can match my voice.
9. A photo of the cats, with a one-line description, and what caption I'd put under it.
10. The GitHub Pages address I'll publish at, so every absolute URL in the head points there.
11. A working title for the page in the same spirit as "Operation Luna Landing," or tell me you'll propose three.

## What to keep from the old page

Keep the whole interface and behavior: the loading screen with the house, the opening note as a pop-up on first visit with the sparkle send-off and a "Read more" link afterward, the Good to know expanders, the sort options (score, cost, cost with discount, name), the schematic map with rings for walking minutes and numbered dots that follow the sort, the score-against-cost chart behind the Map toggle with clickable dots, the filters with single threshold sliders and the value bubble, the reset confirmations, the short list toggle and bottom sheet with its own sort, the hide-a-building toggle with the poof animation, the per-building notes box, the review score that blends Google with ApartmentRatings and discounts small samples (explain the method in Good to know as the old page does), and the fact that everything the reader changes is saved in the browser. Don't remove features; re-point them.

Change what's specific: the title, the hook line, the opening note, the "Winter is when to sign" section (check whether the seasonal pattern holds in this market before keeping it), "Walk away if," "Already ruled out," the questions to ask every building, the building data, the map coordinates (place every building by its real direction and walking time from my address), and the footer's sources and date. Replace every dog-specific thing with the cat equivalent: does the building take cats at all, how many pets, cat deposit, one-time cat fee, monthly cat rent, declaw or indoor-only rules. Keep the "takes them in writing / not confirmed / sources disagree" pill logic. Keep the cost model: twelve months of rent minus advertised free months, plus pet rent, required building fees, one-time fees spread across the year, and the utilities they'd pay themselves, with a stated estimate when nothing is included; the no-deal number stays the headline on each card.

## Photo and share image

Resize the cat photo to about 700 pixels on the long side, compress it to under 100 KB, and embed it as a data URI in the opening note with my caption, the way the old page embeds the dog photo. Remove the old dog photo entirely. Regenerate the share image (1200 by 630) with the new title, a one-line description, the cat photo in the round frame, and the house. Rename it to match the new title and update og:image, twitter:image, og:url, canonical, og:title, og:description, the meta description, and the page title. Keep the house favicon.

## How to work once the interview is done

- Research neighborhood by neighborhood with the same fields the old page uses for every building: name, address, management, year built, unit and size, base rent, listing links, what utilities are included, monthly fees, current deals with conditions, one-time fees, air conditioning and heat type, in-unit laundry, walk time to my address and to transit, Google rating and count from the building's own profile, ApartmentRatings score and written-review count (say whether it's survey-based), recurring review themes, and the cat policy in full. Mark estimated versus verified, and date the data.
- After each pass, fold the buildings into the page's data, keep a ruled-out list with reasons, and re-check that the map has no overlapping labels, the filters' defaults make sense for this price range (tight enough that four to eight buildings show), and the score threshold default sits near the list average.
- Before you hand it back, run the checks the old page went through: the HTML parses with no unclosed tags, the script has no errors in a headless browser, nothing overflows at 360, 390, and 1280 pixels wide, every dialog button works inside a sandboxed iframe (click handlers, not form submits), a full reset returns the page to first-visit state, and the design detector flags nothing. Tell me what you verified and what you couldn't.
- Deliver the same four files the old repo had: `index.html`, the share image PNG, `README.md` rewritten for this search, and `.nojekyll`.
- Voice rules for anything I'll be reading or sending: no em dashes, no filler words, short sentences mixed with longer ones, define local jargon the first time it appears, and say plainly when something is a guess.

When you're done, give me a short list of the buildings that cleared the filters, the one you'd call first and why, and anything I need to confirm by phone before they apply.

Start the interview with question 1.
