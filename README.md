# ReLEAF to Paris

GEMS Taiwan · ReLEAF dashboard for the last stretch of iGEM 2026: the calendar from wiki freeze to the
Grand Jamboree final day (13–16 November 2026, Paris Convention Centre), the hour-by-hour Jamboree plan,
booth shifts, every prep link, the packing lists and Paris travel notes.

Live: https://timmy97-tw.github.io/releaf-jamboree/

One page, `index.html`, no build step and no external requests. All data sits in the script block near the
bottom (`CAL`, `DAYS`, `ROLES`, `MAT`, `LINKS`, `GOALS`, `TASKS`, `ROOMS`); edit those arrays and push.

The two maps are pre-drawn SVGs in `img/` (`paris-map.svg`, `hood-map.svg`) with their pins and route in the
`CITY` and `HOOD` objects. Streets, shops and restaurants come from OpenStreetMap (October 2026); the red dots are
the precisely placed reports in the 19 October snapshot of franceriot.xyz (15–19 October unrest). The booth clip
in `media/` is last year's booth at the 2025 Jamboree.

Sources: the team calendar, `2026 Paris itinerary.xlsx` (Itinerary, Material list, Booth Roster) and
`10_25 Important Links.docx`. Venue and transport details are from jamboree.igem.org/2026/info.

Preview a moment in time with `?now=`, e.g. `?now=2026-11-14T10:30:00%2B01:00` shows Saturday booth duty live.
