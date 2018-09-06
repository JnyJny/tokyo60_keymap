## Firmware

Your Tokyo60 keyboard is a little computer device that needs a program
to run called "firmware". Because reasons. And the keyboard keymap is
part of that program. So everytime you modify the keymap, you need to
rebuild the firmware. Luckily there are lots of easy ways to do that
now and the following describes how to build custom Tokyo60 keymaps
using these tools:

* [QMK Configurator][qmk conf]
* [QMK Toolbox][qmk toolbox]

### TL;DR

1. Download and install [QMK Toolbox][qmk toolbox] for your operating system.<p>

1. Use the [QMK Configurator][qmk conf] to define keycodes in your keymap.
   * Read the [docs][qmk keys] to learn about keycodes.
   * Your keymap should define **L_SHIFT**, **R_SHIFT** and **PAUSE**
   * There is no **FN** key for function, try **MO(1)** instead.
   * Give your keymap a name to make it easier to find.
   
1. Click **Compile**, wait and then **Download Firmware**.
   
1. Start **QMK Toolbox**
   * Click **Open** and select your downloaded firmware.
   * Select **atmega32u4** in the microcontroller pulldown menu.
   
1. Put your Tokyo60 into boot loader mode using **L_SHIFT+R_SHIFT+PAUSE**.
   * The default keymap defines **PAUSE** as **FN+p**.
1. You should see "DFU  device connected" in **QMK Toolbox**.
1. Click the **Flash** button in QMK Toolbox.
1. Wait for a "device disconnected" message.
1. Test out your new keymap!

### It Did Not Work
If your keymap doesn't work or the bootloader key combo,
**L_SHIFT+R_SHIFT+PAUSE** stops working, don't **despair**!

Get out your trusty Philips screwdriver and take the bottom plate off
your keyboard.  With the keyboard upside down, the purple reset button
is on the right hand side in the middle of the board. With **QMK Toolbox**
running and the keyboard plugged in, push and release the reset button
and you will see a device connected message.

Go back and check your keymap to make sure you have a **L_SHIFT**, **R_SHIFT**
and **PAUSE**. 

[qmk conf]: https://config.qmk.fm/#/tokyo60/LAYOUT_60_hhkb
[qmk docs]: https://docs.qmk.fm
[qmk keys]: https://docs.qmk.fm/#/keycodes
[qmk toolbox]: https://qmk.fm/toolbox
