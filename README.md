Update 2026-10-01: Before you print/order anything, read carefully! 

**While working on laying out the pinout for the display converter board i stumpled upon a massive oversight i've had from the very beginning. The Framework motherboard only delivers 2 edp lanes on the IPEX connector. The LP079QX1 display however absolutely needs 4 lanes. In conclusion the attempt, driving the ipad mini 2 display directly off the motherboard can't work.** 

**What does that mean for the entry? The project with its 22cm form factor is still fine with an edp-lvds converter board and an ipad mini 1 display. For me, i've already ordered the ipad mini 2 display. And since my sons can't eat LCD displays, i wont order any more in the foreseeable future.** 

**What happens to the iPad mini 2 display approach? I'll work on an alternative version which will be a little wider, as much wider as the framework extension cards are long. One of the USB-C ports will then be routed internally as usb-c alternative mode with 4 lane edp output and the other USB-C port will be able to take a framework extension card. Though this alternative version would violate the requirements of the design challenge as it would use up one of the 4 ports.** 

**This wider model won't fit onto a 22cm print area, which is very unfortunately. However it gives me more room to align the controls comfortably.** 

**I am exceptionally annoyed by myself, that i didn't catch this oversight early on. Yet i'll make the best out of it.** 

**2026-10-02: and another slap to the face. The ipad mini 2 display arrived. And it doesn't fit the dimensions i've got from googling. I have to update the display holder as well as the gamepad shells to account for the screw holes. Also, since this project starts to get very complicated with planned iterations and alternations, i plan on running a github repository next to the files uploaded to printables. This way you may have complete changelog along the updates. Also there will be a folder struckture to account for compatibilities between iterations (18650 cell bottom, 22cm outer shell and larger shell for ipad 2 display).** 

# Frame Pad - Modular Framework 12 Handheld 

A 3D-printable, modular handheld gaming enclosure designed for the Framework 12 motherboard and battery. 

Ever since the Framework team announced their 16" model with a dedicated GPU i wanted to build a handheld from it, to build the most powerfull handheld gaming console of the world. Though that hardware is way too expensive for me. 

So i was very excited to see this design challenge. Model wise the thing is finished to a point that a first prototype could get assembled. I want to adress some things with further modifications, see TODOs. I've taken all considerations on space for extra electronics, tolerances and modularity for different appliances (e.g. different displays, different gamepad mcu). I'd really love to put a board with current gen. iGPU into it and see how it performs. I've printed the first 2 

iterations of the shell to make sure everything fits but i don't own the hardware for it yet (display connector, ipad mini 2 display and universal battery connectors are ordered). 

More extensive documentation and assembly guides are attached to the files in german and english language. 

**Disclaimer** : The use of these files and instructions is at your own risk. I assume no liability for any damage to hardware or persons resulting from the use of the printed models or the instructions. 

## Design Goals 

- **Full Modularity** : Easy to repair and modify without scrapping the whole case 

   - Also if you want to use a different display, just alter one single module 

- **Print-Friendly** : Optimized for easy printing **with barely any supports needed** 

- **Dual airflow:** no matter if you play in bed or have it on your lab, it will draw fresh air 

- and protect the battery from RAM & CPU heat 

- **Customizable** : Modular fan grid for personal design touches 

- **Accessible** : Uses widely available components (e.g., RP2040 & LP079QX1 [iPad Mini 2/3] 

- Display) 

## Project Status & Disclosure 

This project was created as part of a **Design Challenge** . **Please note:** I do not personally own the Framework 12 motherboard; the design is based on the official STEP files by the Framework team. The full source files (STEP & Plasticity project) will be uploaded immediately after the challenge ends. 

## What do you need to build it yourself? 

- 10x M3 threaded inserts 

- 4x M3x20mm Screws (without the grips) 

- 6x M3x5-6mm Screws 

- 11x M2 threaded inserts 

- 2x Nintendo Joy Con compatible analog joysticks 

- 14x 6*6*4.3mm tactile pushbuttons with SMD feet 

- Solder equipment and experience 

- Cables (for the battery should be at least 1mm² as there is up to 3A across 2 cables, the gamepad wires may be thinner) 

- Universal laptop battery connectors with 2mm spacing and 8 pins (connect battery to motherboard) 

- Breakout board for onboard USB (pogo connectors) and 30 pin 81465-100B-02-D display connector is still to be developed 



## Roadmap 

### TODOs / what's missing and will be done 

- Rework of shoulder buttons, they work but they don't feel comfortable 

- Integrate speakers (-> motherboard pogo connector) 

- Grab USB interface (-> motherboard pogo connector) 

- refine 3d printable pogo connector (motherboard needed) 

- create wiring diagram for display breakout, USB breakout and speakers 

- Create display breakout board (with backlight boost converter) 

- Implement interface cable for battery spacing (universal battery connectors with 2mm spacing should fit) 

- Publish QMK Gamepad Firmware on GitHub 

Nice-to-haves / what's missing and might be done by me 

- Custom 18650 battery pack with RP2040 smart battery driver (would replace bottom shell and interface layer and have a hull around 18650 cells for grips) 

- Attachable grips for more comfort 

- Integration of display touch input (through a touch interface sheet and USB controller propably) 

- tiltable display or kickstand 

## Updates / Changelog 

- V0.1 - initial upload 

- V0.2 - all updates before design challenge ends 

- V0.3 - updates after design challenge ends 

- V1.0 - major release when everything sits 

### 26.09.2026 - V0.2 

- made the power button and spacing in bottom shell larger 

- fixed spacing of interface for the larger power button 

- added Bottom shell with integrated support (0.2mm spacing from shell) 

- Increased holes in left and right gamepad shells for assembled joysticks to go through 

### 28.09.2026 - V0.2 

- many new photos for documentation and actual print added 

- new instruction style in english (just the beginning yet) 

   - feel free to leave feedback on improvements 

30.09.2026 - V0.2 

- fixed many tolerances of controls and threaded insert holders for interface 

- fixed orientation of gamepad shells 

- step files (printables doesn't accept .plasticity files, will upload to github) 

What am i currently working on by priority? / sneak peak 

- Pogo interface to get 3.3V, USB lane and ground to the gamepad 



It will have 1mm diameter solid core wires tightly set and will sit inside the interface sheet for easy assembly. 

- Still rework of shoulder buttons. The one currently on the model are way too small and umcomfortable 

- alternative 8" Turx Display turn cover as the interface board for ipad mini 2 display will need a lot of R&D but i want the first version up and running as fast as possible. I **will** still work on the ipad mini 2 display adapter (shoutout to Elliot Bradley for his great idea with the spring loaded worm screws) 

### **AI Disclosure** 

I've used AI to get my crazy thoughts into a readable text form though the 3d files themself have been made 100% by hand. 

- Documentation, item card & Instructions: Gemma 4 31B 

- Configuration QMK Firmware: Qwen 3.8 & Gemini 

- Post processing of cover image: Gemini 
