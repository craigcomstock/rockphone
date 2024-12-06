# rockphone

A phone which tries to reconcile my love hate relationship with mobile computing technology. Will be as open source as possible both software and hardware. In the shape of a small rock!

# manifesto

Make a phone that is a small, very solid, rock-like object. Something that feels very natural and calming to the touch and fits nicely inside of a pocket, on your wrist with a strap, or up to your ear to listen discretely via bone conduction.

This will be your mobile generic computing device with wireless connectivity anywhere. Stay in touch if you need to, or stay out of touch most of the time to get some peace. 

# specs

- LTE/5G seems a hard requirement in 2024, I have found T-Mobile service nearly requires it
- voice, sms, mms
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

At this point I have been pursuing three separate paths:

- research 5g modules similar to quectel eg-25 in pinephone
  - or maybe find a standalone smartwatch to hack
  - timex familyconnect senior watch was for about a year recently my dream devices nearly
    - termux-app as home made the watch a console watch
    - termux-api hacked for sms/mms allowed cli messagimg
    - simplemessenging app hacked as launcher with a terminal button was primary setup
    - 
- prototype user interface for android
  - simple UI https://github.com/craigcomstock/termux-app/tree/gesture
    - gesture recognition
    - two-line terminal mode (question/answer) prepares for voice interaction
  - command line sms/mms: https://github.com/craigcomstock/termux-api/tree/smsmms-send-receive

- postmarketos on various devices
  - gesture input on linux framebuffer https://gitlab.com/unrznbl/gesture/
  - linux framebuffer "UI" https://gitlab.com/unrznbl/shelli/

# abandoned strategies

- mediatek reverse engineering and such
  - port nuttx-bb (osmocom-bb baseband + posix OS) to MediaTek chipset(s) (6260/6261 are 2G, others 3G+)
  - re-work fernvale open source hardware into the rockphone form factor
  - develop console/speech user interface on top of nuttx-bb
  - develop simple-as-possible manufacturing plan for actual device
  - try to keep device cost as low as possible, goal right now is $35
