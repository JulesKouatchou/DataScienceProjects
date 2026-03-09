## Tracking the movement of the International Space Station

We created a Python tool that tracks the movements of the 
International Space Station (ISS). 
The tool performs the following tasks:
- Do web scraping to extract ISS ephemeris: future positions every 4 minutes over 15 days.
- Convert x/y positions into latitude/longitude coordinates.
- Determine all the individual orbits.
   - `We have a new orbit any time the ISS crosses the International Date Line (180th meridian).`
- Do time interpolation on each orbit to have data points at a frequency as low as 5 seconds
  (instead of 4 minutes as in the initial data).
- On each orbit, determine the country name and the type (ocean or land) of each location.
- Generate statistical data to identify:
   - The total number of orbits.
   - All the countries visited (and how many times)
   - Etc.
- Create various visualization
   - Map the orbits over any visited country
   - Take an arbitrary orbit, color the visted countries and display their flags.
   - Etc.
- Select a random orbit:
   - Do web scraping to get weather prediction data along the orbit
   - Create interactive visualization with weather information on each orbit land grid point.

The tool runs through a Streamlit dasdboard. 
It can complement the [NASA's Spot the Station] (https://www.nasa.gov/spot-the-station/) initiative
and can serve as an educational tool.

The work was accepted for presentation at:

- [PyCon US 2024](https://github.com/astg606/pycon/tree/main/year2024/poster)
- [PyCon US 2025](https://github.com/astg606/pycon/blob/main/year2025/poster/README.md)
