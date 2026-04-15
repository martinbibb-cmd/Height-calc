# Height-calc

A lightweight standalone **Building Height Check** app for estimating building height from:

- manual distance input (distance to wall base)
- captured base angle
- captured top angle

Core formula:

`H = d * (tan(theta_top) - tan(theta_base))`

## Run

Open `index.html` in a browser.

## Workflow

1. Enter distance to base of wall (metres, m)
2. Capture base angle
3. Capture top angle
4. Calculate estimated height

Includes validation and confidence guidance.

When using motion capture, use the on-screen scope reticle and keep the device screen vertical to stay level.
