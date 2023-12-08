# Viper
Build blog of Viper MK1, my own take on a cyberdeck

# General idea
Some characteristics:
- Based on ARM, Raspberry Pi 5 seems a good candidate and it's launching this year apparently.
- Screens! Maybe two of them.
- Slim thingy, smaller than my GPD WM2.
- Mech keyboard? Ortholinear? Hot-swappable switches? Definitely, something with QMK.
- 3D printable case.
- As modular as I can make it.
- I'd like it to have SDR and funny accesories. It should be a fun project.

# Designing the keyboard
Well, I just finally got my 3D printer. It's been a long time wanting one, but the time has come. I've been printing the usual for a week and now the tinkering itch has hit me. I think it's time to start designing a keyboard for this thing, as I think its size will be one of the main limitants of the general size of the device.

I have an idea: design a 3D printable plate as smaller as posible on which I can put Kailh Choc switches. Standard kailh keycaps are a bit bigger than the switches, I'll take a look at that later.

I think I can fit it with enough precision that the switches won't fall. As I don't really want to design a PCB at this time, I think this will be my first take on a hand-wired keyboard too.

So, I've been measuring a Kailh choc v1 with a caliper and translated dimensions to a Fusion360 sketch. 

![Model](https://github.com/0xlillith/Viper/blob/main/img/1.png)

Also made some holes so the keycap's clip can actually... clip. And extruded it all to form some kind of switch socket.

![Model](https://github.com/0xlillith/Viper/blob/main/img/2.png)

I've made some of the measurements bigger to factor in printing tolerances. Some quick prototyping really helps in this.

![Model](https://github.com/0xlillith/Viper/blob/main/img/3.jpg)

I'm really surprised of the precision this thing can print with. I'm using a Bambulab X1C with the 0.2mm nozzle, 0.06mm layer height and PLA material.

The third prototype was the first one to actually click! Also, ejecitng the switch is easy using a standard switch puller.

![Model](https://github.com/0xlillith/Viper/blob/main/img/4.jpg)

Parametrization makes turning an individual socket into a mostly finished plate a breeze.

![Model](https://github.com/0xlillith/Viper/blob/main/img/5.png)

Pending thing is modifiying this to fit some (yet to be found) compatible Mill-Max sockets to where the copper legs are.
