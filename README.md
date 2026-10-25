# ReLEAF to Paris

GEMS Taiwan · ReLEAF dashboard for the last stretch of iGEM 2026: the calendar from wiki freeze to the
Grand Jamboree final day (13–16 November 2026, Paris Convention Centre), the hour-by-hour Jamboree plan,
booth shifts, every prep link, the packing lists and Paris travel notes.

Live: https://timmy97-tw.github.io/releaf-jamboree/

One file, `index.html`, no build step and no external requests. All data sits in the script block near the
bottom (`CAL`, `DAYS`, `ROLES`, `MAT`, `LINKS`); edit those arrays and push.

Sources: the team calendar, `2026 Paris itinerary.xlsx` (Itinerary, Material list, Booth Roster) and
`10_25 Important Links.docx`. Venue and transport details are from jamboree.igem.org/2026/info.

Preview a moment in time with `?now=`, e.g. `?now=2026-11-14T10:30:00%2B01:00` shows Saturday booth duty live.
