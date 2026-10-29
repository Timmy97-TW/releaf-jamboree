# ReLEAF to Paris

GEMS Taiwan · ReLEAF dashboard for the last stretch of iGEM 2026: the calendar from wiki freeze to the
Grand Jamboree final day (13–16 November 2026, Paris Convention Centre), the hour-by-hour Jamboree plan,
booth shifts, every prep link, the packing lists and Paris travel notes.

Live: https://timmy97-tw.github.io/releaf-jamboree/

One page, `index.html`, no build step. The only external request is the Paris weather forecast
(Open-Meteo, at the hotel, cached for an hour); without it the trip-week strip shows November averages. All data sits in the script block near the
bottom (`CAL`, `DAYS`, `ROLES`, `MAT`, `LINKS`, `GOALS`, `TASKS`, `ROOMS`); edit those arrays and push.

English and Traditional Chinese: fixed text carries its Chinese in a `data-zh` attribute; text the script builds
goes through `L(en, zh)` or the `ZH` dictionary (`tx()`). The choice is remembered per browser and defaults to
Chinese when the browser language is Chinese.

The two maps are pre-drawn SVGs in `img/` (`paris-map.svg`, `hood-map.svg`) with their pins and route in the
`CITY` and `HOOD` objects. Streets, shops and restaurants come from OpenStreetMap (October 2026); the red dots are
the precisely placed reports in the 19 October snapshot of franceriot.xyz (15–19 October unrest). The booth clip
in `media/` is last year's booth at the 2025 Jamboree.

The What to bring pictures are Wikimedia Commons photos with the backgrounds cut out; authors and licences are in
`img/bring/CREDITS.md`.

Sources: the team calendar, `2026 Paris itinerary.xlsx` (Itinerary, Material list, Booth Roster) and
`10_25 Important Links.docx`. Venue and transport details are from jamboree.igem.org/2026/info.

Preview a moment in time with `?now=`, e.g. `?now=2026-11-14T10:30:00%2B01:00` shows Saturday booth duty live.
