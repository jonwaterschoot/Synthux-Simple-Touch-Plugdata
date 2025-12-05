# SamplrSeq Touch

Made for Synthux Simple Touch

A basic sampler records 4 samples, short 1 second, with 4 knobs controlling their pitch / speed.
A simple pseudo-randomized sequencer plays a step sequence using the right slider to select different patterns.

> [!NOTE]
> Work in progress - still experiencing pops and crackles.
> More controls could be added to make the seq more interesting

## P10 turn on recording mode

- led starts blinking in a pattern (🐛 = not active on first two presses)
- while recording is active touch pads 4, 6, 8 and/or 9 to record the incoming audio to the buffers
- audio is triggered by a threshold, there's a slight envelope at the beginning and end
- toggle rec P10 off to enter play mode

## Touchpads 4 6 8 9 play samples

- while touched the sample plays until released
- 🐛 trying to resolve the pops when starting touch and releasing the pads

## knob 0 audio input volume

- this will also influence playback volume and recording threshold

## knobs 1 2 3 4 pitch speed

- pitch / speed playback of each sample
    - knob 1 = P4
    - knob 2 = P6
    - knob 3 = P8
    - knob 2 = P9

## knob 5 sequencer tempo

- currently unlinked to any external source so no in or output atm

## fader left - volume out

- volume out, currently no compression or clipping (though clipping is applied to the recorded signal)

## P11 - toggle sequencer

- starting the sequencer will blink the userled in tempo

# fader right - sequencer random seed

- pseudorandom as the fader actually sends values to random seed, which then makes the random pattern repeat exact. If you hit the exact spot again on the fader you would get back the same pattern.
- pattern is 8 steps
    - random triggers 1 of 4 pads for each step
        - I could maybe link a toggle switch to change length from 4 - 8 - 16
        - use second toggle to select sparser or random chance?

- 🐛 not a bug but i'd like to juice up the pattern somehow, e.g. swing or repeats / stutters / chance


--

### unused pads: 0, 1, 2, 3, 5, 7
### unused toggles 
