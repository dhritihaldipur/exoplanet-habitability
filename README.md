# Finding Earth's Twins: Ranking Exoplanets by Earth-Likeness

Which known exoplanets are most similar to Earth? I used real data from the
NASA Exoplanet Archive to rank rocky planets by how close they are to Earth
in size, temperature, and starlight received.

## How it works
1. Cleaned the NASA data and kept rocky planets (radius 0.5 to 1.6 Earth radii)
2. Measured each planet's gap from Earth in radius, temperature, and insolation
3. Converted each gap into a 0 to 1 similarity score: 1 / (1 + gap)
4. Averaged the three scores into one Earth-likeness score and ranked the planets

## Result
Top 5: Teegarden's Star b, TOI-700 d, Kepler-1649 c, Wolf 1069 b, TOI-700 e

## Limitations
This is a similarity score, not proof of habitability. It ignores atmosphere,
water, and stellar activity, and it weights all three features equally.

## Tools
Python, pandas, matplotlib, seaborn (Google Colab)
