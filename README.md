# blackhole
Cinematic black hole featuring customizable settings and perspectives. 

It is a single-file HTML page that renders a cinematic black hole scene in your browser (cinema-inspired).

It includes:
- A **true black** event horizon (stays black no matter what)
- A glowing golden **accretion disk** (golden color when cinematic mode is off)
- **Horizon sparks** that stay “attached” to the disk (don’t drift away when you move the view)
- Subtle **cinematic post effects** (bloom + grain)

No install. No build tools. Just one `.html` file that works.

---

## What you need

- A modern browser with **WebGL2** support  
  (Chrome / Edge / Firefox / Safari, recent versions)

---

## How to run it

### Option A: Open the file directly
1. Save the file as `cinematic_black_hole.html`
2. Double-click it to open in your browser

If your browser blocks local graphics features, use Option B.

### Option B: Run a tiny local server (recommended)

#### Using Python
1. Open a terminal in the folder that contains the HTML file
2. Run:

    python -m http.server 8000

3. Open in your browser:

    http://localhost:8000

4. Click the HTML file in the list

---

## How to use (controls)

### Mouse / trackpad
- **Drag** = pan (move the camera)
- **Scroll / pinch** = zoom

### Keyboard
- **Space** = pause / play
- **H** = hide / show UI
- **F** = focus horizon
- **R** = reset view

---

## UI controls (plain meaning)

- **Zoom**: how close you are to the black hole  
- **Inclination**: tilts the disk (more tilt = more dramatic “side view”)
- **Mass**: changes the black hole size and how strong the lensing feels
- **Lens**: extra lensing strength (higher = more warped light)
- **Disk intensity**: brightness of the glowing disk
- **Disk radius**: how far the disk extends outward
- **Disk thickness**: how “thick” the disk band looks
- **Horizon anomalies**: adds unstable distortion close to the horizon
- **Horizon sparks**: turns the spark details on/off
- **Sparks**: how strong the sparks are
- **Bloom**: how much glow spills into nearby pixels (cinematic glow)
- **Speed**: how fast the scene flows/spins
- **Quality**: image sharpness vs performance  
  - Ultra = best look, more GPU  
  - Performance = fastest, softer image

---

## Sharing a specific look

This page stores a **seed** in the URL hash, like:

    #seed=123456789

- Click **New seed** to get a new look
- Copy the URL to share the exact same look with someone else

---

## Tips

- If performance drops: lower **Quality** or **Bloom**
- For an “Interstellar” vibe, try:
  - Inclination: **60–75°**
  - Bloom: **1.0–1.6**
  - Lens: **1.0–1.3**
  - Sparks: **0.7–1.3**

---

## Troubleshooting

### “WebGL2 not supported”
Try a different browser or update your current one.

### It looks too bright / too dim
Adjust **Disk intensity**, **Bloom**, and **Lens** until it fits your screen.
