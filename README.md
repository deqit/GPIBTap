This adapter started as a way to poke around inside a GPIB‑to‑USB and ‑ethernet adapter (USBGPIB v2 and GPIBee), but it quickly turned into a small side quest to relearn GPIB itself. I have a few GPIB‑enabled instruments on the shelf, and I wanted to finally put them back to work. The last time I seriously touched GPIB was somewhere around 1995, so this felt like a fun way to reconnect with some classic lab tech.

The result is a fully transparent GPIB pass‑through adapter that lets you “listen in” on the bus without interfering. Every GPIB line is broken out twice on pin headers, making it easy to hook up a logic analyzer and start decoding what’s going on. Devices behave exactly as if the adapter wasn’t there.

For quick sanity checks, ATN and REN each get their own LED. The board needs an external 5 V supply for these.

The GitHub repository (see the link on the left) includes everything needed to reproduce the project: schematics, PCB files, and 3D‑printable STLs for a simple enclosure and a small cap for the exposed GPIB-connector-pins. Useful for preventing accidental short circuits when you've got a lot of stuff lying around your desk.

If you want to build one yourself, some SMD‑soldering skills are required. This is very much a DIY project, I don’t have plans to sell kits.

A handy little tool for debugging, reverse‑engineering, or just rediscovering what your GPIB gear has been doing all these years.

This project on Hackaday.io: https://hackaday.io/project/205600-gpib-eavesdropper
More about UsbGpib v2 and GPIBee: https://github.com/xyphro/UsbGpib