# rockphone
A 100% open source phone... in the form of a small rock!

# manifesto
Make a phone that is a small, very solid, rock-like object. Something that feels very natural and calming to the touch and fits nicely inside of a pocket, on your wrist with a strap, or up to your ear to listen discretely via bone conduction.

This will be your mobile generic computing device with wireless connectivity anywhere. Stay in touch if you need to, or stay out of touch most of the time to get some peace. 

# specs
MediaTek 6260/6261/??? core processor for 
- 2G/3G/4G/LTE/??? 
- SIM card slot
- SD card slot
- headset jack (optional)
- wifi
- bluetooth for audio, serial console, more
- qi charging
- bone conducting exciter so you can put the rock up to your temple/ear and do a voice call or interact with the device via voice, discretely
- microphone
- some subtle lighting, like maybe one glowing RGB light where color indicates different states
- some simple capacitive or resistive touch for simple gestures or handwriting recognition
- accelerometer for movement gesture control

# carrying options
- bare, in your pocket
- in a watchband
- on a necklace

# slogans
- "Hold your head up!" -from the band Argent song... no screen... no need to wander around looking down.
- "A Personal Journey" -contrasting this device with cloud-based language parsing and interactions... this device will by default not use the cloud but rather develop with the individual user.

# technical plan
- port nuttx-bb (osmocom-bb baseband + posix OS) to MediaTek chipset(s) (6260/6261 are 2G, others 3G+)
- re-work fernvale open source hardware into the rockphone form factor
- develop console/speech user interface on top of nuttx-bb
- develop simple-as-possible manufacturing plan for actual device
- try to keep device cost as low as possible, goal right now is $35
