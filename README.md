# mouSTer

*When someone is a mouse master. He's very good with mouse, instead of keyboard.
You call that person a mouSTer.* [^1].

***
![mouSTer logo](/assets/images/mouSTer-logo.svg)
## mouSTer is a universal USB HID class device to db9 adapter.
### mouSTer is the first fully configurable USB adapter for old computers.
***
### Supported Platforms:

- Atari 400, 800, XL, XE
- Atari 260ST, 520ST, 1040ST(e) 
- Atari 2600
- Atari Falcon
- Atari VCS
- Commodore 64 
- Commodore Amiga (500,600,1000,1200,2000,3000,4000)
- Commodore Amiga CD32
- Commodore VIC-20
- ZX Spectrum via Kempston Interface

 ###### ... and probably much more.
 ***

### mouSTer can emulate:

- Atari mouse 
- Amiga mouse (need a min rev. 0.8.298 [driver](https://github.com/willyvmm/Amiga-mouSTer-wheel-mouse-driver/releases/latest) and min firmware rev. 3.20.4600 for wheel support)
- Joystick
- Gamepad
- Commodore C1351 mouse (GEOS mouse)
- Trackball (experimental)
- new, non yet existing devices :)
***
### Supported USB[^2] Devices:

- ALL USB mouses
    - literally ALL
- ALL USB Gampads
    - literally ALL or almost ALL
- ALL USB Joysticks
    - USB joysticks are not so popular, so **mouSTer** has not been tested with too many of them.
***
### Unsupported USB Devices:

-  "Keyboard Point Stick for Lenovo IBM Thinkpad Computer" - a trackpoint clone
***
### mouSTer features:

- full configurable
- easy firmware update via USB Memory
- adjust the mouse speed
- full support for button mapping
- full support for autofire on ANY button
- autofire speed is also configurable
- built-in debug feature, allowing the collection of debug data in case of troubles.
***
## Notes about Amiga driver and protocol:

The protocol has been designed to ensure minimal code footprint and quick processing keeping high compatibility with classic mouse.
Unfortunately, the protocol relies on CIA clock, and will not work on systems with overclocked CIA.
The main clue of the protocol is to be as much compatible with the standard as possible.
So far, the driver do not hijack any buttons, so both LMB and MMB may be used without any issues. 
However, there is ONE buttons combination that is not supported:
Simultaneously pressing LMB + MMB disables receiving new wheel events from the mouSTer.

#### Features:
- Vertical wheel support
- Horizontal wheel support
- Mouse button #4 support
- Mouse button #5 support

#### Technical details:
 TBD.
***
### mouSTer history:

![mouSTer pac](/assets/images/mouSTer_pac.jpg)

mouSTer was born as a **hid2st** device around autumn 2013. The first hardware revision was based on the almost unknown **FTDI Vinculum II** (VNC2) chip. Unfortunately, that was the worst development decision ever. I would say that was a shoot to the knee at the beginning of the journey. Don't touch this chip.
Since then the hardware platform changed three times, and around autumn 2018 the mouSTer got its final physical shape. On the other end - the firmware went through the same bumpy way. 
- 4 hardware revisions and 3 times firmware revisions made from scratch.
- the latest 3.x firmware has 17 major revisions and has circa 4000 effective code lines + libraries (at the time of writing)

#### The mouSTer Family

![The mouSTer Family](/assets/images/mouSTer_family.jpg)

***
### mouSTer is leading the way.

I may proudly say, the shape that the **mouSTer** presents has been unofficially adopted as a standard.
There are more devices shown up on the market recently that use the same physical shape. Also, some firmware features were successfully adopted in other products.
###### So ... stay tuned. More to come.
***

### Future development

| Activity | status |
| --- | ---| 
| New Amiga driver | ![](https://geps.dev/progress/100) |    
| New Atari 8bit pointing device | ![](https://geps.dev/progress/95) |    
| Support for Apple Desktop Bus emulation |  ![](https://geps.dev/progress/25) |
| Support for PC Serial mouse emulation | ![](https://geps.dev/progress/37) |
| Support for SEGA Mega Drive pad emulation | ![](https://geps.dev/progress/10) |
| We're open to suggestions | ![](https://geps.dev/progress/999) |
| Open source wheel driver for Amiga | ![](https://geps.dev/progress/34) |
| Semi-open SDK for your emulation | ![](https://geps.dev/progress/1) | 
| Let us know if you're interested | ![](https://geps.dev/progress/100) |
| So we can prioritize tasks| ![](https://geps.dev/progress/70) |

***

## Firmware download
### Latest stable firmware download: https://github.com/willyvmm/mouSTer/releases/latest
Please do not use the 3.16.2600 release. It's buggy. instead please use this: https://github.com/willyvmm/mouSTer/releases/tag/3.17.3475 or newer until the new stable firmware is released.
### Latest pre-release (if any) can be found here: https://github.com/willyvmm/mouSTer/releases/

***

## Where to buy

* https://retrohax.net/shop/modulesandparts/mouster/
* https://retrolemon.co.uk/atari-st-ste-falcon/133-mouster.html
* https://www.ebay.de/itm/324483346054
* Contact US if You want to be here.

***

## Community support us - We support community
* [Mega65](https://mega65.org/)
* [SillyVenture](https://www.sillyventure.eu/)
* [TeddyBeer C64](http://teddybeer.party)
* [This Week In Retro](https://open.spotify.com/episode/3X6t5OdsUFIq29dhtJoK28)
* [flashjazzcat](https://www.youtube.com/watch?v=1FINefdkQls)
* [tahustvedt](https://cults3d.com/en/users/tahustvedt/creations) - [3D printed case](https://retrohax.net/wp-content/uploads/2021/03/Mouster-case.zip)
* [CTRL-ALT-REES](https://www.youtube.com/watch?v=DwwULPDCpWE) - [CTRL-ALT-REES](https://www.youtube.com/watch?v=xk1SMQ9HkBY)
* [MR.Lurch](https://www.youtube.com/watch?v=YkYoK3WywfU)
* [RetroGralnia](https://www.youtube.com/watch?v=TnNj3VBJfCA)
* [Hackaday](https://hackaday.com/2020/07/14/modern-mice-on-old-computers/) - [Hackaday](https://hackaday.com/2021/01/22/mouster-brings-usb-to-retro-computers/) - [Hackaday](https://hackaday.com/2021/08/09/this-old-mouse-building-a-usb-adapter-for-a-vintage-depraz-mouse/) - [Hackaday](https://hackaday.com/2023/02/16/the-mouster-adapter-now-has-amiga-scroll-support/)
***
## Meet us on Discord [![](https://dcbadge.vercel.app/api/server/UcGMrMgv7V)](https://discord.gg/UcGMrMgv7V)
***
[^1]: https://www.urbandictionary.com/define.php?term=Mouster
[^2]: Device with wireless adapter connected to USB port is still USB Device. 
