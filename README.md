# rave-maria-II
Let's rebuild the iconic Rave Maria, this time as a melody-generator

One 320 x 240 TFT touchscreen (HSD028309 B34, [ili9341 driver](https://github.com/lvgl/lvgl/blob/master/docs/src/details/integration/external_display_controllers/ili9341.rst))

Two potentiometers

Variables to control:
- BPM (also controlled via cv)
- Meter
- Number of measures
- Scale
- Note Density per measure (ranging from one whole note per measure to 16 16th notes, deconstructing bigger notes in some clever, random way)
- Note range (from every note being the same, to every note being chosen from 8, or 12, or 32 or whatever different possibilities up and down the scale)
- Melodic complexity (what are the chances of large skips or jumps between neighboring notes)
- MIDI out channel
  - What if it also played bass? We'd need a channel for that, too
  - Could something cool happen with MIDI in?!
- Start
- Stop
- Emergency off (note off all channels)
- Create new melody
- Save melody?
- Transition to new melody?
- Chance to start replace notes at random

So at the end of the day, you could push a few buttons on the touch pad and spin a few knobs, and get an eight-measure 4/4 melody at 120 bpm, where each measure was likely to have three quarter notes and two eigth notes (but might have more or less) and each note was likely to be only a step away from its neighbor, but could be a little more or a little less. It would send the notes to be played by a synth (and maybe generate a bass line that would get played by a different synth) and over time, each note would be replaced by a different one.
