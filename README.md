# Event Horizon

A real-time black hole ray tracer that runs in the browser. One HTML file, WebGL2, no libraries or build step.

Open `index.html` in a browser that supports WebGL2.

## What it does

- Traces each pixel's light ray backwards along its Schwarzschild geodesic, using the orbit equation u″ + u = 3⁄2 u² (u = rₛ/r).
- Corrects camera directions into the local frame of a hovering or radially free-falling observer, including aberration.
- Renders a thin accretion disk with a Novikov–Thorne temperature profile, Keplerian Doppler beaming and gravitational redshift. Disk color is Planck's law at the shifted temperature.
- **Fall in** (key `F`): radial free fall through the horizon, with live readouts for clock rate, tidal stretch and proper time left.
- A 2D diagram of ray deflection near the critical impact parameter b = 3√3⁄2 rₛ.
- Physical numbers for Cygnus X-1, Sgr A*, M87* and TON 618, plus predicted shadow sizes compared with Event Horizon Telescope measurements.

## Limits

- The black hole doesn't spin (Schwarzschild, not Kerr).
- The disk is thin, with procedural texture.
- Light travel time isn't modeled.
- The disk temperature slider sets the look; it isn't a physical value.
- Masses and distances are literature values that haven't been re-checked against current sources.

## Hosting

To publish it, enable GitHub Pages (Settings → Pages → deploy from `main`, root).
