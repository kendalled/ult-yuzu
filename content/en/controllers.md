---
title: Controller Setup
description: 'Information on setting up controllers in Parsec & Yuzu.'
position: 5
category: 'Resources'
---

Information about setting up the most common controllers on Parsec & Yuzu.

<alert type="info">
  Plug in your controller (and adapter / software if needed) before starting Yuzu or Parsec. This ensures everything works correctly.
</alert>

## Official Nintendo Adapter & GameCube Controller

If you intend on playing via Parsec (online), you need a program to convert your GameCube controller inputs to Xbox 360 inputs. I recommend [Delfinovin](https://github.com/Struggleton/Delfinovin/releases/download/v0.02/Delfinovin.zip), but there are many options. Delfinovin is made by one guy, is proven to be safe, and works every time.

### How to use Delfinovin

- Close Parsec, Yuzu, Steam, etc. (anything that can use controller inputs)

- Click Delfinovin.exe in the folder where you saved it

- A black box should pop up with 4 options. Press 1 and then enter to start the controller loop (reads GameCube controller). You should see numbers and at this point if you press buttons on the controller you should see all of the values change. If not, see the video guide below.

<alert type="info">
  If you try running Delfinovin and it seems to crash, follow <a href="https://www.youtube.com/watch?v=bi2hf6VxmiI" title="Video Guide to Fix Delfinovin" target="_blank">this guide</a> <b>exactly</b>.
</alert>

If you made it this far and you see your controller's inputs in the black box, continue below.

### Fix button layout in Parsec

- You only have to do this step <b>once</b>. It will make your life easier. Start Parsec without connecting to your host. Go into Parsec Gamepad settings, and unmap `Back`. Then, map the `Z` button on your controller to Right bumper. Finally, swap A & B. 

### Yuzu settings

- Start Parsec & connect to your Host. 

- Once they are in Yuzu, have them select "xInput Controller 0" as Player two, and make your left stick's range 60%.

- Enjoy playing!

<alert type="warning">
  You must fix your left stick's range (60%) in Yuzu <i>every time</i>. This is because everyone you connect to has a different copy of Yuzu and it doesn't save your controller settings. If buttons aren't behaving as they should, see the button layout section above.
</alert>



## Third Party Adapter & GameCube Controller

Check the [Yuzu documentation](https://yuzu-emu.org/wiki/faq/#how-do-i-use-my-gamecube-controller-adapter) for more information about installing and using GameCube controllers with Yuzu. MayFlash and 8BitDo adapters are the easiest to configure. If you are using a Mayflash or 8BitDo adapter, simply switch it to PC mode and it will work natively. If your third party adapter does not have a PC mode, I am unsure and the steps below may work but are not guaranteed.

## Nintendo Pro Controller

Simply plug in your Pro Controller to your PC with a USB-C cable to get started. No configuration is required besides going into Yuzu and clicking `Emulation > Controls > Connect Controller` in the top left.

