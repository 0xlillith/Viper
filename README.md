# Viper
Build blog of Viper MK1, my own take on a cyberdeck

![til](https://github.com/0xlillith/Viper/blob/main/img/0-blog-barney.gif)

# General idea
Some characteristics:
- Based on ARM, Raspberry Pi 5 seems a good candidate and it's launching this year apparently.
- Screens! Maybe two of them.
- Slim thingy, smaller than my GPD WM2.
- Mech keyboard? Ortholinear? Hot-swappable switches? Definitely all of them, also something with QMK.
- 3D printed case.
- As modular as I can make it.
- I'd like it to have SDR and funny accesories. It should be a fun project.

# Designing the keyboard
Well, I just finally got my 3D printer. It's been a long time wanting one, but better late than never. I've been printing the usual benchy and prebuilt goodies for a week and now the tinkering itch has hit me. I think it's time to start designing a keyboard for this thing, as I think its size will be one of the main limitants of the general size of the device.

## Keyboard Plate

I have an idea: design a 3D printable plate as smaller as posible on which I can put Kailh Choc v1 switches. Standard kailh keycaps are a bit bigger than the switches, I'll take a look at that later.

I think I can fit it with enough precision that the switches won't fall. As I don't really want to design a PCB at this time, I think this will be my first take on a hand-wired keyboard too.

So, I've been measuring a Kailh choc v1 with a caliper and translated dimensions to a Fusion360 sketch. 

![Model](https://github.com/0xlillith/Viper/blob/main/img/1.png)

Also made some holes so the keycap's clip can actually... clip. And extruded it all to form some kind of switch socket.

![Model](https://github.com/0xlillith/Viper/blob/main/img/2.png)

I've made some of the measurements bigger to factor in printing tolerances. Some quick prototyping really helps in this.

![Model](https://github.com/0xlillith/Viper/blob/main/img/3.jpg)

I'm really surprised of the precision this thing can print with. I'm using a Bambulab X1C with the 0.2mm nozzle, 0.06mm layer height and PLA material.

The third prototype was the first one to actually click! Also, ejecting the switch is easy using a standard switch puller.

![Model](https://github.com/0xlillith/Viper/blob/main/img/4.jpg)

Parametrization makes turning an individual socket into a mostly finished plate a breeze.

![Model](https://github.com/0xlillith/Viper/blob/main/img/5.png)

Fits very well!

![Model](https://github.com/0xlillith/Viper/blob/main/img/6.jpg)

Pending thing is modifiying this to fit some (yet to be found) compatible Mill-Max sockets to where the copper legs are.

UPDATE: I'm kinda deciding against hand-wired now, probably  wiser to design a PCB and send it to pcbway.

## Keycaps

So, I wanted to try and print my own keycaps. I spent an afternoon smashing all buttons at once in front of fusion and some crazy designs came out. At the end, tho, I decided in favor of a more generic spherical profile, similar to DSA but a lot smaller and slim. I spent the next morning playing with the printer and got something similar to a doubleshot keycap... I will call this profile the DoubleHot.

All this testing was done using grey PLA, next thing is to print this in dual color ABS and then try to acetone-smooth it.

Turns out the ABS filmanent I got (official Bammbu's) has low Styrene content and this has a side effect of it not being suitable to acetone smoothing. All my testings where failed. Also, apparently my precision printing ABS was worse than with PLA so... back to PLA!.
I've also been testing diverse fonts and decided to use Routed Gothic for a classy look.

Current best keycap printing settings:
- PLA
- Cold Plate
- 0,2 nozzle
- 0,06 layer height
- Support yes, normal, auto, snug.
- Print Sequence: By Object.
- Sparse infill 40% rectilinear.
- Print in vertical, 90º. Way better than horizontal, safer than 45º.

Post-Processing:
- Currently, no sanding. No acetone.
- Just finishing with some lacquer. I like Montana Colors Acrylic - Matte.

# Mouse
Want to try an integrated mini trackball.

# SBC
Just got the Raspberry Pi 5! Installed the official cooler and the RTC battery, a 128GB SD and installed Kali to do some testing with it. Everything seems snappy and fine.

# Screen
Got 2 ultrawide 8" from Taobao, with MIPI connection plus an mHDMI board. Idea is to mount one screen over the other, and make them stack when closed.
I intend to connect both of them to the RPI using MIPI flex cables. Just discovered an adapter cable is needed. RPI5 has 2 4-rail connectors, each of them can be connected to a camera or a screen. This connectors use mini-FPC format, 22 lanes and 0,5mm wide. There are adaptor cables to connect them to the standard 15 lanes and 1mm wide.

# Power
I think a stack of generic rechargeable batteries is ideal.

# Internal USB
Gotta investigate some USB hats.

# Chassis
3D Printed, I suppose polyamide or polycarbonate are firm candidates, but i've never used them for now.

# SDR
An integrated HackRF won't probably fit, it's too big.


