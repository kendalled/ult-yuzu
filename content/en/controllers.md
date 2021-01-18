---
title: Controller Setup
description: 'Information on setting up controllers in Parsec & Yuzu.'
position: 5
category: 'Resources'
---

Information about setting up the most common controllers on Yuzu.

<alert type="info">
  Plug in your controller (and adapter / software if needed) before starting Yuzu or Parsec. This ensures everything works correctly.
</alert>

## Third Party Adapter & GameCube Controller

Check the [Yuzu documentation](https://yuzu-emu.org/wiki/faq/#how-do-i-use-my-gamecube-controller-adapter) for more information about installing and using GameCube controllers with Yuzu. MayFlash and 8BitDo adapters are the easiest to configure. If you are using a Mayflash or 8BitDo adapter, simply switch it to PC mode and it will work natively. If your third party adapter does not have a PC mode, I am unsure and the steps below may work but are not guaranteed.

## Official Nintendo Adapter & GameCube Controller

If you intend on playing via Parsec (online), you need a program to convert your GameCube controller inputs to Xbox 360 inputs. I recommend [Delfinovin](https://github.com/Struggleton/Delfinovin/releases/download/v0.02/Delfinovin.zip), but there are many options.

### How to use Delfinovin (what makes your Nintendo Adapter work)

- Close Parsec, Yuzu, Steam, etc (anything that can use controller inputs)

- Click Delfinovin.exe in the folder where you saved it

- A black box should pop up with 4 options. Press 1 and then enter to start the controller loop (reads GameCube controller). You should see numbers and at this point if you press buttons on the controller you should see all of the values change. If not, see the video guide below.

- Start Parsec & enjoy playing

<alert type="warning">
  If you try running Delfinovin and it seems to crash, follow <a href="https://www.youtube.com/watch?v=bi2hf6VxmiI" title="Video Guide to Fix Delfinovin" target="_blank">this guide</a> <b>exactly</b>.
</alert>


## Nintendo Pro Controller

Simply plug in your Pro Controller to your PC with a USB-C cable to get started. No configuration is required besides going into Yuzu and clicking `Emulation > Controls > Connect Controller` in the top left.

