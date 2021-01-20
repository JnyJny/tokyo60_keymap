# 1UP Keyboard RGB 60% HTE™ (Hotswap Tsangan Edition)

I bought a [1UP 60% Hotswap Tsangan Edition PCB][0] (1up60hte) to
replace a USB-C version of the Tokyo60 PCB with an intermittant fault
in the USB connector. The price of the 1up60hte was comparable to the
Tokyo60 and had the same feature set (RGB, HHKB compatible, USB-C
connector). Various internet reports indicated this board would work
in a Tokyo60 chassis.

I am happy to report the 1up60hte fits my season one Tokyo60 chassis
perfectly; all internal mount points had corresponding through-holes
for screws and all hotswap pockets lined up with the Tokyo60 top
plate. It's a solid replacement, physically. 

The 1up60hte board has a silver reset button located on the bottom
of the board, located near the space bar. This button is used to
place the board into DFU mode to flash on new firmware. 

The board arrived with firmware installed, which seemed to be the
[Tsangan layout][1]. The Tsangan layout differs slightly from the
[HHKB][2] layout (left/right control in R4). At the time of this
writing, selecting the HHKB layout would result in an empty keymap
(all the keys were present, but not assigned keycodes). It's just
a matter of assigning keys to the keymap, but still sort of inconvenient.

I was able to flash the 1up60hte the firmware generated from this
[keymap layout][3] without difficulties.


[0]: https://www.1upkeyboards.com/shop/controllers/1up-rgb-60-pcb-hte/
[1]: https://config.qmk.fm/#/1upkeyboards/1up60hte/LAYOUT_tsangan
[2]: https://config.qmk.fm/#/1upkeyboards/1up60hte/LAYOUT_60_hhkb
[3]: https://github.com/JnyJny/tokyo60_keymap/blob/master/firmware/1up60hte_keymap.json

