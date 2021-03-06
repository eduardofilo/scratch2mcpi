## Scratch2MCPI(Scratch2MinecraftPi)

[日本語の情報](http://scratch2mcpi.github.io/)

With Scratch2MCPI, you can control [Minecraft Pi Edition](http://pi.minecraft.net/) from [Scratch](http://scratch.mit.edu) on Raspberry Pi.

On the latest 2.0, it supports Minecraft Graphics Turtle.

[Demo Movie](https://www.youtube.com/watch?v=w9lkdCEPKWc) on YouTube

## Installation

Install Minecraft Pi Edition if you don't have. You can either install from http://pi.minecraft.net/?p=68 or use the following installation script.(If you install Raspbian OS from the latest NOOBS, Minecraft Pi may be pre-installed. If the Minecraft Pi icon exists on the Desktop, skip this step.)

```
$ curl http://scratch2mcpi.github.io/mcpi.sh | sh
```

Install Scratch2MCPI

```
$ curl https://raw.githubusercontent.com/eduardofilo/scratch2mcpi/master/install.sh | sh
```

## Getting Started

1. Start Minecraft, click "Start Game", then "Create New". Wait until the new world is generated.
2. After the world is generated, double click Scratch2MCPI icon to start Scratch and Scratch2MCPI.
3. On Scratch, click Green flag, and run the script. "hello minecraft" should be displayed on Minecraft chat window.

## How to use

You can send the following commands by "broadcast" block of Scratch.

- `hola_minecraft`: Send "hello minecraft" message to chat section.
- `escribe <mensaje>`:
- `ponPos`: Move the player to the position specified by Scratch variables: "mcpiX", "mcpiY", "mcpiZ".
- `ponBloque`: Place the block at the position specified by Scratch variables: "mcpiX", "mcpiY", "mcpiZ". The block type and block data can be specified by Scratch variables: "blockTypeId" and "blockData".
- `ponBloques`: Pone bloques entre las posiciones especificadas por las variables Scratch: "mcpiX1", "mcpiY1", "mcpiZ1" y "mcpiX1", "mcpiY1", "mcpiZ1". The block type and block data can be specified by Scratch variables: "blockTypeId" and "blockData".
- `leePos`: Get the current position of the player. The position values can be gotten by Scratch sensor values: "PlayerX", "PlayerY", "PlayerZ".
- `leeAltura`: Get the y position of the highest block at the position specified by Scratch variables: "mcpiX" and "mcpiZ". The y postion can be gotten by Scratch sensor value "posY".
- `leeToquesBloque`: Get the block event information of the last block hit by the player. The event info values can be gotten by Scratch sensor values: "blockEventX", "blockEventY", "blockEventZ", "blockEventFace", "blockEventEntityId".
- `leeBloque`: Obtiene la información del bloque situado en la posición especificada por las variables Scratch: "mcpiX", "mcpiY", "mcpiZ". El tipo y dato del bloque se almacena en las variables Scratch: "blockTypeId" y "blockData".
- `limpia`: [WARNING] Reset the world. This will delete clean up the world, so please be aware to use it.
- `util:dibujaEsfera`
- `util:dibujaCirculo`
- `util:dibujaLinea`
- `util:dibujaCara`
- `util:limpiaPuntosForma`
- `util:ponPuntosForma`

## Reference

- [Minecraft API](http://www.stuffaboutcode.com/p/minecraft-api-reference.html)

## Requirements

- [scratchpy](https://github.com/pilliq/scratchpy)
