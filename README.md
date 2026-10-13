# SOS 110 · In-Class Review Assignment 2: Mapping a Biogeochemical Cycle

A five-slide web deck for the in-class hand-off of In-Class Review Assignment 2.

**Live:** https://ryanpcornell.github.io/sos110-review-assignment-2/

1. **Title**
2. **Announcements**: upcoming assignments, plus a live attendance roll call the
   instructor runs from the `?host` copy of the deck.
3. **The assignment**, set as a course handout: objective, the cycle and context
   choice, the three sections (Title, Diagram, Summary), and submission.
4. **Before You Upload**: the student self-assessment checklist beside the
   drawing conventions (stock, flow, cloud, + / − arrow, human touchpoint).
5. **★ Cycle Systems Builder**: a stock-and-flow and causal-loop builder for one
   biogeochemical cycle, with per-cycle palettes, feedback-loop detection, a model
   run with and without human impacts, Save / Open (a `.cycle.json` file), an
   autosave in the browser, and **Save as PDF** in the assignment's three sections.

The builder also runs on its own at
https://ryanpcornell.github.io/sos110-cycle-systems-builder/ (same browser
autosave, so work started on one opens on the other).

Everything is self-contained: no build step, no dependencies, no media folder.
The only external requests are Google Fonts.

## Running it in class
Open the live link. Press <kbd>→</kbd> / <kbd>space</kbd> or click to advance;
<kbd>M</kbd> or the ☰ button opens the slide menu. Add `?host` to the URL for the
instructor copy, which gets the **Attendance** button on slide 2.

## Built from
`_deck-builder/review2_assignment.py` + `_deck-builder/review2_cycle_builder.py`
(not in this repo; this is the built output).

`firebase-config.js` holds the Firebase web config and the attendance endpoints.
Those values are not secrets: they ship in every web page that uses them, and
access is controlled by the Firestore security rules. No student data is written
to Firestore; attendance goes straight from the browser to a Google Form, and the
builder stores nothing anywhere but the student's own browser.
