---
title: In Game Reset (IGR)
subtitle: Executable ELF That Returns Memory Card Emulator Devices to their assigned Boot Card.
description: Executable ELF That Returns Memory Card Emulator Devices to their assigned Boot Card and Restarts the PS2. (MCP2)[https://qrco.de/bdiiDa], [SD2PSX](https://sd2psx.net/), [PSXMC2](https://www.bitfunx.com/product/psxmemcard-gen2-memory-card-for-playstation1-ps-one-playstation2-game-consoles/), [PSXMC](https://a.co/d/cD5wr0u), [PMC](https://www.psx-place.com/threads/picomemcard-a-cheap-diy-memory-card-with-usb-to-transfer-saves-to-pc-and-store-multiple-images.37515/), etc.)
developer: JonathanDotCel
visit_project: https://github.com/JonathanDotCel/bootcard_igr
hide_hero: true
sysapps_code: SAL001-005
layout: sysappslist
image: https://s33.postimg.cc/xlv59493z/IGR_BG.jpg
version: v0.1
features:
    - label: Compatible across all models
      icon: fa-user-check
    - label: Updated sometimes
      icon: fa-file-upload
    - label: Fairly popular
      icon: fa-chart-line
download: https://app.filen.io/#/d/1da94440-50c7-47ce-a9b4-15fd223b03af#2kqIHZ70G83uSv5Oq1CPzu9h1bKEteq7
rating: 5
---

An IGR (intergrated reset) binary, which will mount your default <MCE (Memory Card Emulator)> Boot Card and restart the PS2.

Most commonly used in 2 ways:

1: Use it as your `IGR.ELF` for OPL

In OPL Settings, set your In-Game-Reset path to `mc0:/SYS_IGR/IGR.ELF` or `mc1:/SYS_IGR/IGR.ELF` (mc0 for slot 1, mc1 for slot 2)
OPL will launch it when you hit the In-Game-Reset Key Combination (Unless you have Enabled Mode 6 in Game Settings), Pressing L1 + L2 + R1 + R2 + select + start in-game will stop a game and launch the ELF you set for IGR path, which will switch the MCE device back to it's assigned Boot Card, and then restart the PS2.
This is especially useful for using the Game-ID Card Switching feature of MCE devices, as it will bring you back to your FMCB/PS2BBL/Tuna card when exiting a game.

2: Install it as a FMCB menu item with Free MCBoot Configurator

If you have multiple cards with exploits on them on your MCE and want to quickly get back to Boot Card, this would allow you to do so. Simply add it to the cards that need a way back to Boot Card, and map the addition with Free MCBoot Configurator.
Scroll to it and hit `X` when FMCB starts to load your default Boot Card on the MCE Device.
