# 南宫阙 Look Mechanics

## Natural motion

南宫阙 is a humanoid cultivator with a separate head and neck, physical eyes, a rigid hairpin, paired earrings, gathered hands, wide sleeves, and a long grounded robe. Her gaze should remain poised and authoritative.

- Anchor both feet, the lower robe, waist, and gathered hands to one stable baseline and body registration.
- Let the complete physical eyes lead: irises, pupils, eyelids, eye whites, and highlights change together inside the original almond-shaped apertures.
- Follow with restrained head yaw or pitch, then a very small neck and upper-shoulder response.
- Preserve skull, brow, nose, mouth, forehead mark, and facial spacing without stretching or broad raster warping.
- The rigid hairpin follows the head as one attached object. Earrings remain attached and may lag by only a very small, continuous amount.
- Wide sleeves and hands stay calm and connected. Lower robe volume and character scale remain stable.
- Never rotate, skew, tilt, or slide the entire sprite to fake gaze. Do not replace the approved slim almond eyes with round eyes.

## Cardinal pose families

- `000 up`: pupils and irises move clearly upward within both almond eyes; upper eyelids open slightly, chin lifts modestly, forehead and nose remain centered, torso and feet stay fixed.
- `090 screen-right`: pupils, irises, nose tip, and face aim unmistakably toward the image-right edge; head yaws right with a restrained three-quarter cue, while the opposite cheek becomes more visible. Hairpin follows the head; earrings remain attached.
- `180 down`: pupils and irises move clearly downward; upper eyelids lower slightly, chin tucks toward the collar, forehead mark remains centered and readable, torso and feet stay fixed.
- `270 screen-left`: pupils, irises, nose tip, and face aim unmistakably toward the image-left edge; head yaws left with the opposing three-quarter cue. Hairpin follows the head; earrings remain attached.

Intermediate directions interpolate evenly between these pose families. Diagonals must visibly carry both required axes. Screen-left and screen-right are viewer/image coordinates, never character-relative coordinates.

## Motion budget

Each 22.5-degree step changes eye direction first, then head yaw/pitch by a small even increment, with only restrained neck/shoulder follow-through. Adjacent steps keep the same head size, body height, foot baseline, lower-robe anchor, hand position, sleeve attachment, hairpin structure, and facial proportions. The `157.5 -> 180`, `337.5 -> 000`, and row boundary transitions must be one ordinary step with no snap, scale pop, side flip, or prop jump.
