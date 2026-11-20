# Gemini 4 Neon: prompts

Each prompt is sent once to Gemini 4 Neon and once to Claude Fable 5.2. Zero retries, default settings.

## Test 1: Wow output
Build a single self-contained HTML file (three.js from a CDN is the only dependency): a night-time Kathmandu rooftop scene. Prayer flags ripple in the wind, the Boudhanath stupa glows in the distance, lanterns drift upward, and the camera does a slow cinematic orbit. Add soft bloom, realistic fog and a day/night toggle. No external assets; everything is procedural. Make it look like a film still.

## Test 2: 1-minute reel
Create a 60-second vertical (1080x1920) motion-graphics film as one self-contained HTML file, styled like a premium Instagram Reel. Vanilla JS with Canvas 2D, SVG and CSS; GSAP from a CDN is the only allowed dependency. No images or external fonts.

Story: "The Life of a Prompt". One sentence is typed on a phone, travels across the world to a data centre, gets broken into tokens inside a model, and comes back as an answer.

Style: bold flat motion design. Three colours only: ink #0B0B0F, lime #C6FF3D and paper #F4F1EA. Heavy sans-serif type, thick strokes, hard cuts. No gradients, glows, particle clouds or lens flares.

Timeline (exact):
0-2s HOOK: the word "ENTER" slams in at full width, the screen shakes, then a hard cut.
2-10s: a thumb types "make me something amazing" on a minimal phone. Every letter pops with squash and stretch.
10-20s: the sentence peels off the screen, becomes one line, and draws a route across a stylised world map to a data centre.
20-32s: inside the model, the words split into token blocks that stack, shuffle and lock into a grid while a token counter ticks up.
32-44s: the answer builds word by word as kinetic typography, every word landing on the beat.
44-54s: a speed-ramped montage of 6 quick 1.5s stat cards with numbers counting up.
54-60s: the line from the map draws the end card "One prompt. One minute." then loops cleanly back to the first frame.

Motion rules: every transition is a match cut or a mask wipe built from the previous scene's shapes. Use expo and back easing, overshoot and secondary motion. Something moves at every moment, and no text holds still longer than 1.5s. Captions are big enough to read on a phone, with 120px safe margins at the top and bottom.

Audio: a 120 BPM beat generated with Web Audio (kick, hat, and a riser before each cut), with cuts landing on the beat. A Play button starts it, a thin progress bar runs along the bottom, and R restarts. It must hold 60fps and play exactly the same way every time, so it can be screen-recorded.

## Test 3: Single-HTML explorable 3D world
Build "Himalayan Village": a single self-contained HTML file (three.js from a CDN is the only dependency). A procedural mountain valley with terraced fields, a river, stone houses with smoke from the chimneys, prayer wheels you can click to spin, and a day/night cycle. First-person WASD + mouse-look controls, with collision with the ground. Show an FPS counter. No assets loaded; everything is generated in code.

## Test 4: SVG attention-hijack
Create one SVG (no external fonts or images): a pelican riding a bicycle through a neon city at night, with motion lines, reflections on wet asphalt and a glowing "NEON" sign. Use gradients, filters and SMIL animation so the wheels spin and the sign flickers. It should be striking at thumbnail size.

## Test 5: Technical
One of these three tracks; the results name which one was run.
- **A. Real bug fix:** a real failing issue from an open-source repo. Pass if the patch passes the tests on the first try.
- **B. Long-context needle:** paste ~500K tokens (several books or docs) with 5 planted facts and ask for all 5 with locations. Score n/5 and measure the time.
- **C. Agentic tool use:** 10-step task with function calls (search, then compute, then write a file). Score the steps completed without help.
