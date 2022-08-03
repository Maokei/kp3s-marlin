# kp3s-marlin
Marlin configuration for Kingroon KP3s FDM 3D-printer.

## Additional
- Modified version of the `MKS Robin Nano` board named `KingRoon KP3 v1.2`
- Screen modified MKS TFT24 -> Kingroon TFT24 v1.1
- Drivers `TMC2225` drivers which are compatible to `A4988`

## How to build

### How to build (VSCODE)
- Install [Visual Studio Code](https://code.visualstudio.com/Download)
- Install [PlatformIO Visual Studio Code Extension](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide)
- Install [Auto Build Marlin Extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=MarlinFirmware.auto-build).
- Run command `git clone git@github.com:MarlinFirmware/Marlin.git`
- Enter source folder `cd Marlin` and `git checkout bugfix-2.1.x`
- Copy configuration from this repository `Configuration*.h` to the folder `Marlin` inside the clone firmware repository (`/Marlin/Marlin`)
- Follow [Auto Build Marlin](https://marlinfw.org/docs/basics/auto_build_marlin.html) usage instructions.

## How to flash
- Rename BIN file that was generated `Robin_nano.bin` location: (VSCODE method location `Marlin/.pio/build/mks_robin_nano35/Robin_nano35.bin`)
- Copy bin file to SD-card root
- Insert SD-card into printer and start it up.
