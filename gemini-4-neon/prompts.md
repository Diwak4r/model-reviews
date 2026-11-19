# Gemini 4 Neon: prompts

Each prompt is sent once to Gemini 4 Neon and once to Claude Fable 5.2. Zero retries, default settings.

## Test 1: Wow output
Build a single self-contained HTML file (three.js from a CDN is the only dependency): a night-time Kathmandu rooftop scene. Prayer flags ripple in the wind, the Boudhanath stupa glows in the distance, lanterns drift upward, and the camera does a slow cinematic orbit. Add soft bloom, realistic fog and a day/night toggle. No external assets; everything is procedural. Make it look like a film still.

## Test 2: 1-minute showreel
Create a 60-second animated showreel as one self-contained HTML file (canvas or three.js from a CDN) that plays automatically: 6 scenes of 10 seconds each, with smooth transitions, kinetic typography introducing "Gemini 4 Neon", a particle morph, a 3D product-style spin of a glowing logo, a data-viz scene and a final title card. Include a visible timeline bar. It must be screen-recordable at 1080x1920 (vertical).

## Test 3: Single-HTML explorable 3D world
Build "Himalayan Village": a single self-contained HTML file (three.js from a CDN is the only dependency). A procedural mountain valley with terraced fields, a river, stone houses with smoke from the chimneys, prayer wheels you can click to spin, and a day/night cycle. First-person WASD + mouse-look controls, with collision with the ground. Show an FPS counter. No assets loaded; everything is generated in code.

## Test 4: SVG attention-hijack
Create one SVG (no external fonts or images): a pelican riding a bicycle through a neon city at night, with motion lines, reflections on wet asphalt and a glowing "NEON" sign. Use gradients, filters and SMIL animation so the wheels spin and the sign flickers. It should be striking at thumbnail size.

## Test 5: Technical
One of these three tracks; the results name which one was run.
- **A. Real bug fix:** a real failing issue from an open-source repo. Pass if the patch passes the tests on the first try.
- **B. Long-context needle:** paste ~500K tokens (several books or docs) with 5 planted facts and ask for all 5 with locations. Score n/5 and measure the time.
- **C. Agentic tool use:** 10-step task with function calls (search, then compute, then write a file). Score the steps completed without help.
