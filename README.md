# rockphone
A 100% open source phone... in the form of a small rock!

# hardware
Current plan is to prototype a breakout board for the SIM800H and/or MT2502A and proceed from there. These are selected because they both contain the MT6260 which is being opened up by the fernly project.

https://github.com/xobs/fernly

The breakout boards will likely be something that is simple, cheap and easy to experiment with. Either have headers that plug into a breadboard or have a header like is on the Raspberry Pi to breakout via ribbon cable or via adapter to breadboard.

# manifesto
Make a phone that is a small, very solid, rock-like object. Maybe even surround it with some material like concrete. No screen, plugs, wires, outlets, etc... Interaction would be through Bluetooth, WIFI, GSM and a BCE (Bone Conducting Exciter) a sort of speaker you must place against your head to hear well. A microphone would be included somehow. The device would charge via Qi Wireless charging. The device would be somewhat touch sensitive, either just a single area or maybe a complex enough area to recognize simple gestures, possibly even letters.

The idea is to make a very sturdy and right-sized object to carry around in your pocket. If it falls from high, no problem. Also so that it doesn't disturb your life by beeping, buzzing and showing things on a screen.

Inside, the system would primarily be written in Lua (LuaJIT likely to interface well with C libraries/functions) so that it is fairly easy to understand like an old BASIC computer (TRS-80, C64, Apple). When you connect via Bluetooth or WIFI from your computer you are on a console and can do things like text, call, email, etc... you can also write new functions or debug/modify existing functions.

The goal is a 100% open source device. Probable external projects to be used are:

- luajit (for main interface and programming language)
- pocketsphinx (for voice recognition)
- espeak (for speech synthesis)
- python pyo (sound synth library)
- fernly, nuttx, osmocom-bb for eventually driving the open part of the system down deeper into the hardware.

Slogans are
"Hold your head up!" -from the band Argent song... no screen... no need to wander around looking down.
"A Personal Journey" -contrasting this device with cloud-based language parsing and interactions... this device will by default not use the cloud but rather develop with the individual user.
