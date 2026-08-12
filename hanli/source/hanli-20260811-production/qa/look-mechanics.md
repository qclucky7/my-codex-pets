# 韩立 look mechanics

## Identity and scale lock

- Candidate C and the approved idle family are the identity source of truth: young but not childish, calm restrained grey-brown eyes, straight dark brows, slim masculine face, half-up long black hair, horizontal silver-green hairpin, dark emerald wide-sleeved outer robe, pale blue-grey crossed collar, dark belt, and black boots.
- Keep the same roughly three-head-tall chibi proportions, head size, shoulder width, robe length, planted foot baseline, lighting, material detail, and saturated emerald palette as idle.
- The lower torso, robe hem, and feet remain registered. Do not rotate or slide the whole character to fake gaze.

## Natural motion

- Eyes lead the gaze, then the head and neck turn or pitch naturally, followed by restrained shoulder and upper-torso movement. Match the approved row-9 right/up motion language.
- Use controlled three-quarter head yaw for horizontal directions and clear head pitch for vertical directions. Preserve skull volume, slim jaw, facial spacing, narrow eyes, nose shape, mouth, ears, hairline, bangs, and identity; avoid full profile or broad raster deformation.
- Long hair, crown, and hairpin stay attached and retain their design. They follow head motion naturally, with gradual cheek occlusion and no side-flipping or length change.
- The robe, belt knot, sleeve construction, hands, and feet remain stable. No new prop or effect appears.

## Cardinal pose families

- `000 up`: eyes lift, head pitches up, neck follows, with restrained upper-torso response.
- `090 screen-right`: eyes lead and head/neck yaw naturally toward screen-right in a restrained three-quarter pose.
- `180 down`: eyes lower, head pitches clearly down, neck follows, with restrained upper-torso response.
- `270 screen-left`: eyes lead and head/neck yaw naturally toward screen-left in a restrained three-quarter pose that visibly opposes `090`.

## Row 10 motion budget

- Order: `180`, `202.5`, `225`, `247.5`, `270`, `292.5`, `315`, `337.5`.
- `180 -> 270`: lower the gaze first, then increase screen-left yaw in three even steps. Nose tip and both pupils progress from center to the left side of the head.
- `270 -> 337.5`: retain screen-left yaw while lifting the gaze and chin in three even steps. The face approaches the up family but never crosses to screen-right.
- `180` is one even step after existing `157.5`; `337.5` is one even step before approved `000`.
- No neighboring pair may jump in scale, baseline, facial construction, hair volume, robe width, or lighting.
