# ABS on Go2

A quadruped robotics project page covering Go1-to-Go2 adaptation, simulation training, and deployment on a real robot.

This page presents an independent reproduction and engineering application of Agile But Safe. It is not the official project page for the original paper or a complete training code repository.

## Page structure

- `index.html`: A standalone static landing page with real-robot demonstrations before simulation demonstrations.
- Real-robot gallery: Four portrait slots in one row on desktop and two columns on tablet and mobile.
- Simulation gallery: Four landscape slots in a 2 × 2 grid on desktop and one column on mobile.
- Available media can be enlarged by clicking it; press Escape or use the close button to exit.
- Missing media is shown as a placeholder rather than as a completed demonstration.
- `engineering-notes.html`: Preserves the full previous page, including unfinished engineering notes.

## Add eight GIFs

Copy the files into `static/gifs/` using these case-sensitive names. The display order is left to right, then top to bottom:

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

`real` denotes real-robot demonstrations, and `sim` denotes simulations. The page preserves each GIF's original aspect ratio without cropping the subject. All eight display slots are ready, but the final GIFs have not yet been added to this repository.

A local Mac path such as `/Users/...` cannot be used as an image URL on the website. Copy the GIFs into the repository directory above and commit them. You can rename the copies without changing the original files.

The scene titles are neutral numbered labels for now. After reviewing the full demonstrations, update the corresponding `h3`, `data-title`, `aria-label`, and `alt` values in `index.html` if needed. The real-robot and simulation numbers do not imply paired tests under identical conditions. The demonstrations alone do not establish a statistical success rate or performance improvement.

## Local preview

The landing page needs no build tools or third-party CDN. Open `index.html` in a browser, or run `python3 -m http.server 8000` from the repository root and visit `http://localhost:8000`. Placeholders are expected until the final GIFs are added.

## Sources and license

- Original ABS project: https://agile-but-safe.github.io/
- Official ABS code: https://github.com/LeCAR-Lab/ABS
- Original website template, Nerfies: https://nerfies.github.io/

The site is adapted from the Nerfies template. This version reorganizes the landing page and retains attribution to the template. The website retains the [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) license notice. The original algorithm and project remain the work of their respective authors.
