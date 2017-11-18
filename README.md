# Arduino IDE board definition for Multi 4-in-1 transmitter module
At this point the only supported board/module is the Atmega328p-based module, the STM32-based module is not yet supported.

## Installing
The board definition is installed using the Arduino IDE Boards Manager.

1. Open the Arduino IDE
2. Go to File->Preferences (or Ctrl+Comma)
3. Locate the 'Aditional Boards Manager URLs' field and paste in this URL: https://raw.githubusercontent.com/benlye/multi-4in1-board/master/package_multi_4in1_board_index.json
4. Click OK to save the change
5. Click Tools->Board [Board Name]->Boards Manager
6. Scroll to the bottom of the list of boards and click on 'Multi 4-in-1 Boards' then click the Install button
7. Click Close to close the Boards Manager

## Selecting the board
1. Click Tools->Board [Board Name]
2. Scroll down the list to 'Multi 4-in-1 Boards' and select 'Multi 4-in-1 (Atmega328p, 3.3V, 16MHz)'

## Choosing the bootloader
There are two bootloader options.  The default 'No bootloader' won't install a bootloader, allowing the maximum space for protocols.  The 'Optiboot with Boot Delay' option installs a small Optiboot bootloader which is compatible with the Er9x and Ersky9x option to flash firmware from the transmitter's maintenance menu.

1. Click Tools->Bootloader [Bootloader Option]
2. Select the desired bootloader

**Recommended:** Click Tools->Burn Bootloader to set the fuses, even if the 'No bootloader' option was selected.

## Compiling / uploading firmware
Visit the main Multi 4-in-1 module repository for instructions to configure, compile, and upload the firmware

https://github.com/pascallanger/DIY-Multiprotocol-TX-Module/
