I built this adapter while poking around inside a friend’s GPIB‑to‑USB-and‑Ethernet adapters (UsbGpib v2 and GPIBee). The goal was simple: see what’s really happening on the GPIB bus without disturbing it.

The result is a fully transparent GPIB pass‑through that lets you tap every single bus line via pin headers making it easy to hook up a logic analyzer and start decoding traffic. It stays completely out of the signal path, so the device under test behaves as if nothing is there.

For quick visual feedback, ATN and REN each get their own LED. The board needs an external 5 V supply for the LEDs.

The GitHub repo includes everything you need to reproduce it: schematics, PCB files, and 3D‑printable STLs for a simple enclosure. There are caps to cover the exposed GPIB-connector-pins, to avoid accidental short circuits.

A handy little tool for anyone debugging, reverse‑engineering, or just curious about what their GPIB hardware is really saying.