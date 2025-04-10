# THIS IS A SELF-TRIGGERING DISTORTION FX FOR SYNTHUX SIMPLE TOUCH

Made with Plugdata by jonwtr.

After watching the interview between Roey an Nick about how Audrey has -among a lot of other things-  a short delay in the feedback loop, I began experimenting with some of these concepts. That's resulted in now having a filter and a delay in a feedback loop that's passing through the simplest of distortion fx: clipping. By experimenting with the order of the delay/feedback, filter and clipping I landed on this iteration.

Interesting side effect of implementing this principle is that without any real input, the patch starts self oscillating when you hit the sweet spots / threshold of the delay time. Playing with the filter and timing will result in a droning effect.

When using this as a 'regular' distortion you'll probably want to keep the dry / wet value under control. Most often I find the sweet spots in the delay time in the smaller values. Opening up knob 5 and then playing with the right fader multiplier. Once you have a certain sweet spot, you might want to try adding a bit of LFO (knob4).
Sometimes toggling off randomizer P2 but mainly the top pad P11 will keep things at bay.

Also make sure to try out sending different amounts of volume to the input using your other gears output volume.

Please do feel free to further tweak this and let me know what can and should be improved.

## Youtube demo
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/csmBTfaORss/0.jpg)](https://www.youtube.com/watch?v=csmBTfaORss)

https://youtu.be/csmBTfaORss

## QUICK INSTALL
Download the [Binary file](selfdistort_touch.bin) and flash using the [Daisy Seed web programmer](https://electro-smith.github.io/Programmer/)

## CONTROLS
<img src="touch.jpg" width="300"/>

### **Switches**
- S07-OFF-S08 = on/off/on switch: **delay timing** multiplier
    - left: (off) x 1
    - middle: x 0.5
    - right: x 70
- S09-OFF-S10 = on/oof/on switch: trigger pad **distortion values**  multiplier
    - down: x 0.02
    - middle: x 0.4
    - up: x 0.8

### **Knobs**
- S30 Knob 00 - distortion amount
- S31 Knob 01 - pre-distortion filtering sweep between lowpass and highpass
- S32 Knob 02 - distortion DRY / WET
- S33 Knob 03 - post-distortion lowpass filter
- S34 Knob 04 - delay time LFO mix
- S35 Knob 05 - delay time mix
- S36 Fader Left - end of chain volume out 
- S37 Fader Right - delay time multiplier of knob 5
- 
### **Pads**
- P3 > P9 : increasing amounts of distortion - These will add up to each other and to the value set by Knob0 (values will 'fold' back, so adding values will not max out, but might add up to lower values)
- P0 : attack / decay toggle - between long and short for pad distortion triggers P3-P9
    - default short attack and decay = 20ms
    - long attack / decay = 1000ms (1sec)
    - you can release pad before full value is reached
    - holding will sustain to pads max value

- P1 : /
- P2: toggle randomizer for delay LFO
- P10: reset / clear delay buffer
- P11: toggle randomizer delay timing mix



<img src="diagram_sketch.jpg"/>
