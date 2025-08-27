# Frequency shifter - Audio in FX

This is an experimental patch where I was exploring using `[hv.freqshift~]`as a live audio FX.

I also added `[hv.flanger2~]`in the mix.

In short these are the controls of the frequency flanger patch.

in my patches I count knobs from 0 - 5
```
Knob layout:

1 - 2 - 3 - 4
0           5
```

**Slider left**: Main Frequency (0-880)

This slider is modulated and adjusted in this flow:

 - **knob 2**: freqshift mod move 1

 - v v v v 
 
 - **knob 1**: freqshift mod move 1

 - v v v v

 - **knob 0**: stereo shift

 - v v v v

 - **Leftswitch**: freq shift multiplier

 - v v v v

 - **knob 3**: lopass `[hv.lop~]` before the actual freq shift

  - v v v v 

  - actual `[hv.freqshift~]`

It then goes into another lopass:

 - **knob 4**: lopass `[hv.lop~]` after the actual freq shift

This whole chain passes through the flanger block `[hv.flanger2~]`, which is manipulated by different amounts using the touchpads 3 - 9

 - **knob 5**: wet / dry mix

The touchpads don't yet do enough imo.

But the intention was that each pad sends a different amount of the flanger effect, which is in turn randomized by using toggle two.

**Toggle 2:** 
 - up: value 0
 - middle: value randomizer set by a drunk lfo
 - down: combination of numbers from knob2 and a sine osc.
