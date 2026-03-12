# running-pace-calculator
A lightweight running pace calculator that computes time, distance, and pace, with additional metrics like speed and race time predictions.

# PaceCalc — Running Pace Calculator

A clean, mobile-friendly running pace calculator built with vanilla HTML, CSS, and JavaScript. Enter any two of three variables (distance, time, or pace) and the missing value is calculated automatically.

---

## Features

- **Smart calculation** — fill in any two fields; the third is computed for you
- **Race predictions** — instant finish time estimates for 5K, 10K, Half Marathon, and Full Marathon
- **Speed output** — displays your pace in both min/km and km/h
- **Mobile-friendly** — responsive layout that works on any screen size
- **Keyboard support** — press Enter to calculate without clicking the button
- **Zero dependencies** — single HTML file, no frameworks or build tools required

---

## Usage

Open `pace-calculator.html` in any modern web browser — no server or installation needed.

### How to calculate

1. Enter values in **any two** of the three input sections:
   - **Distance** — in kilometers (e.g. `10.00`)
   - **Time** — in `hh : mm : ss` format (e.g. `0`, `52`, `30` for 52 minutes 30 seconds)
   - **Pace** — in `mm : ss` per kilometer (e.g. `5`, `15` for 5:15/km)
2. Click **Calculate** (or press `Enter`)
3. The missing field is filled in and highlighted in blue
4. Results and race predictions appear below

### All three filled in?

If you enter values in all three fields, the calculator will use **distance + time** to recompute pace.

---

## Outputs

| Output | Description |
|--------|-------------|
| Pace | Minutes and seconds per kilometer |
| Speed | Kilometers per hour |
| Distance | Total distance in km |
| Time | Total elapsed time (hh:mm:ss) |
| 5K prediction | Estimated finish time at 5.0 km |
| 10K prediction | Estimated finish time at 10.0 km |
| Half Marathon | Estimated finish time at 21.1 km |
| Marathon | Estimated finish time at 42.2 km |

---

## File Structure

```
pace-calculator.html   # Single self-contained file (HTML + CSS + JS)
README.md              # This file
```

---

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). No polyfills required.

---

## Limitations

- Race predictions assume a **constant pace** — no fatigue model is applied
- Time input does not validate beyond basic range checks (e.g. seconds 0–59)
- Designed for **metric units** (kilometers) only

---

## License

Free to use and modify for personal or educational purposes.
