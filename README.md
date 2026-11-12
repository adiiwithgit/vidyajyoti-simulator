# Vidyajyoti Satellite Simulator

Browser-based simulation of the Vidyajyoti 3U CubeSat (VIT Mumbai), with a deep dive into the Electrical Power System (EPS).

## What it models
- Circular LEO orbit: period, speed, eclipse geometry (cylindrical shadow, beta angle)
- Six subsystems with live power draw: EPS, OBC, COMMS, ADCS, Payload, Thermal
- EPS chain: solar array → MPPT → regulated bus → Li-ion battery
- Orbit-average energy balance, depth of discharge, automatic safe mode below 20% charge

## Run
Open `index.html` in any browser. No build step. Pages: `explorer.html` (3D), `orbit.html` (power simulator), `builder.html` (game).

## Assumptions
Nadir-pointing attitude, 3U body-mounted cells, triple-junction cell efficiency adjustable, MPPT 95%, battery charge/discharge efficiency 95%, no temperature or degradation model yet.

## Ideas for contributors
- Temperature-dependent cell efficiency and battery capacity
- Ground-station passes driving real comms duty
- Panel degradation over mission years
- Compare body-mounted vs deployable vs sun-pointing attitude

## License
MIT
