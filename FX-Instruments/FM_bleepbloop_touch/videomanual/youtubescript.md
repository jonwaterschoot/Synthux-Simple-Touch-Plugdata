# **YouTube Tutorial Script: FM BleepBloop for Synthux Simple Touch**

**Video Title:** FM BleepBloop \- A Free Experimental Sequencer for Synthux Simple Touch (Plugdata/Daisy)

Video Description:  
In this video, I'm sharing "FM BleepBloop," a free firmware I created for the Synthux Simple Touch. It's a fun and chaotic FM synth and sequencer made with Plugdata. I'll show you how it works, what it can do, and how you can install it on your own device\!  
Find the project on GitHub (includes .bin file, .pd patch, and full manual): \[Link to your GitHub\]  
Learn more about Synthux: \[Link to Synthux Website/Discord\]  
Learn more about Plugdata: \[Link to Plugdata Website\]

### **1\. Introduction (Approx. 0:00 \- 1:30)**

**(0:00 \- 0:15) \- \[Fast-paced montage of the FM BleepBloop making interesting sounds. Show close-ups of your hands interacting with the device, the LED blinking, maybe some shots of it synced with other gear.\]**

**(0:15) \- \[Cut to you on camera, with the Simple Touch in front of you.\]**

**YOU:** "Hey everyone, and welcome\! What you just heard is the FM BleepBloop, a little weird untuned synth and sequencer patch I designed for the Synthux Simple Touch. My name is Jon, using the name @jonwtr online, and I'm a huge fan of synthesizers and DIY electronics."

**YOU:** "I'm a volunteer moderator over on the Synthux Discord, and I got into building my own instruments and making music after I became disabled with chronic pain. It's been an amazing creative outlet for me. This project is one of the results of that journey, and I'm really excited to share it with you all."

**YOU:** "In this video, I'm going to give you a tour of how the FM BleepBloop works. We'll take a quick peek at the Plugdata patch behind it, I'll demonstrate all the features and performance controls on the hardware itself, and finally, I'll show you how easy it is to get this running on your own Simple Touch. So, let's dive in\!"

### **2\. The Plugdata Patch (Approx. 1:30 \- 3:30)**

**\[Screen recording of the Plugdata patch. Slowly pan across the main sections.\]**

**YOU:** "Okay, so here's where it all started: the Plugdata patch. For those who don't know, Plugdata is a visual programming environment. It’s fully Puredata compatible, but with a more friendly gui and an inbuild toolchain that allows to save your patches as plugins, or, as in our case here today, as code that can compile onto a Daisy Seed , which is the brain of the Synthux Simple Touch."

**YOU:** "For those who do not know Synthux and the Simple Touch devices: Synthux has built the Simple Touch as an easy gateway into the world of synthesizer building. You can get it pre-built or as a diy kit you solder togheter yourself. It comes with a build guide and a course to get you up and running. There are a few firmwares, fully playable instruments and FX built by one of Synthux’s main coders, Vlad. The code he made is fully available on GitHub, and there is a whole community over at Discord, ready to help, learn and inspire. Simple touch comes with a few faceplates you can swap to fit some of these pre-made instruments.

… Or, you could hack the device, build on top of it and/or write your own code. I’m using plugdata, not always as powerfull as straight up coding, but imo way easier to grasp as a beginner. I also came from using Bitwig and the Grid, I did some virtual patching with the eurorack simulator VCV and even the 3D software Blender which also has a lot of node based patching.”

**YOU:** "Here it is, my patch. As you can see, the patch is... well, it's a bit of a beast\! The core of it is a complex FM oscillator, which I based on a fantastic tutorial by Simon Hutchinson—I'll link to that below. This is what gives the synth its unique, and often unpredictable, character."

**\[Briefly zoom in on the main FM oscillator section, then to the sequencer logic, then to the parameter controls.\]**

**YOU:** "I won't go through every single wire here, but you can see the main sections: we have the FM engine, the controls for attack and decay, the internal 8-step sequencer, and all the logic for handling the touchpads and randomizers."

**YOU:** "Now, I'll be the first to admit, this could be optimized\! I could use more abstractions to clean it up, and I'm still learning as I go. But the great thing is, it works\! And if you're curious, you can download this very patch file from my GitHub. It's a great way to learn and see how things are put together, or even to start tweaking it yourself."

**YOU:** "If you want to get started with Plugdata and the Simple Touch, the Synthux community is the best place to go. They have amazing resources and a super helpful Discord server. I myself built an incomplete guide, and I also saw someone built a similar, cleaner guide. There are some great introduction videos by HVCC’s maintainer Dreamer, aka Wasted Audio, his youtube videos are the best way to get fully introduced into the workings of going from PD to C."

### **3\. Hardware Demonstration (Approx. 3:30 \- 15:00)**

**\[Cut back to you with the hardware. Focus on your hands interacting with the device for the rest of this section. Use picture-in-picture if you want to keep your face on screen.\]**

**YOU:** "Alright, let's get our hands on the hardware, because that's where the fun really is. I'm going to walk you through the controls and modes."

**\[Point to the faders and knobs.\]**

**YOU:** "First up, the basics. The left fader is your master volume, and the right fader controls the tempo of the internal sequencer. These six knobs are where you'll do most of your sound shaping. The first four control the FM parameters—it's best to just twist and listen to what happens. These two are for your Attack and Decay."

**\[Demonstrate twisting the knobs and the effect on the sound.\]**

**YOU:** "Now, for the touchpads. This patch has two main modes: Simple Mode and Array Mode. You can switch between them using this first pad, P1."

**\[Press P1 to toggle modes.\]**

**YOU:** "In **Simple Mode**, you're playing the synth live. The sound you hear is coming directly from the current position of the FM knobs. The seven main pads here will slightly alter the pitch."

**\[Play a bit in Simple Mode.\]**

YOU: "In Array Mode, these seven pads trigger seven different preset sounds. When you first power it on, it loads a set of sounds I've saved, but you can create and record your own."  
\[show the arrays in the PD patch\]  
**\[Switch to Array Mode and play the pads.\]**

**YOU:** "How do you record? Easy. You hold down the 'record' pad, P10, and tap P3 to enter recording mode. Now, in Array Mode, you can dial in a sound with the FM knobs, and then press one of the seven pads to save it to that slot. This doesn't save when you power down, so it's a fresh canvas every time."

**\[Demonstrate recording a new sound to a pad.\]**

**YOU:** "But what if you want instant chaos? Hold P1 and tap P3. This fills all seven slots with completely random FM values. It's a great way to find happy accidents."

**\[Demonstrate the random fill.\]**

#### **The Sequencer**

**YOU:** "Now for my favorite part: the sequencer. To turn it on, you hold P11 and tap P7. It's an 8-step sequencer that plays the pads. It works in both Simple and Array mode."

**\[Turn on the sequencer and let it play.\]**

**YOU:** "You can change the tempo with the right fader. You can also randomize the sequence at any time by pressing the top pad, P0. The two switches at the top give you even more control. The first one changes the sequence length from 8 steps, to 4, to 2\. The second switch controls probability, determining the chance that any given step will play. This is amazing for creating evolving, generative patterns."

**\[Demonstrate the sequencer, the randomizer, and the switches.\]**

#### **FX and Advanced Controls**

**YOU:** "We're not done yet\! There are a bunch of hidden combo-presses for effects and advanced control. The image on the GitHub page is your best friend here."

**\[Briefly show the manual image on screen.\]**

**YOU:** "For example, holding P2 gives you access to FX. While holding it, you can use these pads to add random panning, or these to engage a comb filter for weird, resonant delay effects."

**\[Demonstrate the panning and comb filter.\]**

#### **Syncing**

**YOU:** "And yes, it can sync\! If you've modded your Simple Touch with TRS MIDI, it will respond to MIDI start/stop messages. It also has clock input. But my favorite feature is the audio sync. Hold P11 and tap P5, and it will listen to an incoming audio signal, like a kick drum, and sync its tempo. It works like a tap tempo."

**\[Demonstrate syncing to an external beat from another device.\]**

### **4\. Installation & Outro (Approx. 15:00 \- 17:00)**

**\[Screen recording of the Daisy Web Programmer page.\]**

**YOU:** "So, you want to try this out? It's super simple. All you need is the binary file, which is on the GitHub page. You don't need to touch Plugdata or any code if you don't want to."

**YOU:** "Just go to the Daisy Web Programmer—flash.daisy.audio. Go to the upload tab and select the .bin file I provided on GitHub. Connect your Simple Touch to your computer via USB and put it into bootloader mode by holding the 'Boot' button and then pressing 'Reset', if the bootloader isn’t loaded yet, you could upload via the regular mode as well, just follow the instructions on the the web page, hit 'Program'. That's it\! In a few seconds, you'll be running FM BleepBloop."

**\[Cut back to you on camera.\]**

**YOU:** "So that's the FM BleepBloop. I hope this was helpful and inspires you to make some fun, weird noises. It's been a really rewarding project for me, and I'm so happy to be able to share it with this community."

**YOU:** "If you enjoyed this, please give consider visiting the Synthux channel and join our Discord. All the links to the GitHub, to Synthux, and to Plugdata are in the description below. Go grab the files, experiment, and please let me know what you create with it\! Thanks so much for watching, and I'll see you next time."

**(17:00 onwards) \- \[End with another 15-20 seconds of a cool musical jam using the device, maybe with some other gear. End screen with links to GitHub and other videos.\]**