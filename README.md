# Mars Insolation Project

An interactive simulator of daylight and sunlight on Mars across its eccentric year.

**Live site:** https://alejandrozu.github.io/mars-insolation-project/

Mars has a sol close to an Earth day and an axial tilt close to Earth's (25.19°), but its orbit is far more eccentric (e = 0.0934). The seasons have unequal lengths (154 / 193 / 179 / 143 sols) and sunlight at perihelion is about 45% stronger than at aphelion (713 vs 490 W/m²), so the length and strength of daylight behave very differently from Earth.

## What it does

- **Mars view**: the orbit drawn to scale, with season wedges whose areas follow Kepler's second law, plus a side view of the tilt. A ground view shows the sky dome at any latitude, with sun paths in local true solar time.
- **Daylight duration**, **insolation** (daily mean or peak) and **seasonal ratio** (brightest ÷ dimmest, log scale) across the year for any set of latitudes, or a whole spectrum of them.
- **Circular-orbit reference**: the same planet with e = 0, to isolate the effect of eccentricity.
- **Align southern seasons**: plots southern latitudes from their own winter solstice.
- **Two and three suns**: mirror arrays at the Sun–Mars L4 and/or L5 points, at strengths that can bring the average flux to Earth's level.
- **Earth comparison** lines, Mars or Earth hours, dynamic or fixed axes, and full-screen or compact layouts.

## Model

Keplerian orbit (a = 1.5237 AU, e = 0.0934, perihelion at Ls 250.9°), year of 686.98 days (668.6 sols), top-of-atmosphere insolation from 1361 W/m² at 1 AU, and sunrise when the Sun's centre crosses a flat horizon. Today's Mars date uses the Allison & McEwen (2000) formula. All of it runs in the browser from a single `index.html`, with no build step and no server.
