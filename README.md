# ABS on Go2

A quadruped robotics project page covering Go1-to-Go2 adaptation, simulation training, and deployment on Unitree Go2.

This repository presents an independent reproduction and engineering application of Agile But Safe. It contains the project website, demonstration media, and a technical record of the adaptation; the original ABS project and code are linked below.

## Page structure

- `index.html`: A standalone static landing page with real-robot demonstrations before simulation demonstrations.
- Real-robot gallery: Four portrait rollouts in one row on desktop and two columns on tablet and mobile.
- Simulation gallery: Four landscape rollouts in a 2 × 2 grid on desktop and one column on mobile.
- Demonstrations can be enlarged by clicking them; press Escape or use the close button to exit.
- `engineering-notes.html`: Technical record of environment setup, training, Real-to-Sim calibration, perception integration, and deployment.

## Demonstration media

The eight GIFs are stored in `static/gifs/` using stable, case-sensitive names. The display order is left to right, then top to bottom:

```text
static/gifs/
├── real-01.gif
├── real-02.gif
├── real-03.gif
├── real-04.gif
├── sim-01.gif
├── sim-02.gif
├── sim-03.gif
└── sim-04.gif
```

`real` denotes real-robot demonstrations, and `sim` denotes Isaac Gym rollouts. The page preserves each GIF's original aspect ratio without cropping the subject.

The real-robot cards use neutral numbered titles because they are qualitative Agile Policy deployment rollouts rather than distinct benchmark scenarios. The simulation cards retain descriptive environment names. The real-robot and simulation numbers do not imply paired tests under identical conditions, and the demonstrations are not presented as statistical success-rate measurements.

## Local preview

The landing page needs no build tools or third-party CDN. Open `index.html` in a browser, or run `python3 -m http.server 8000` from the repository root and visit `http://localhost:8000`.

## Sources and license

- Original ABS project: https://agile-but-safe.github.io/
- Official ABS code: https://github.com/LeCAR-Lab/ABS
- Original website template, Nerfies: https://nerfies.github.io/

The site is adapted from the Nerfies template. This version reorganizes the landing page and retains attribution to the template. The website retains the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license notice. The original algorithm and project remain the work of their respective authors.
