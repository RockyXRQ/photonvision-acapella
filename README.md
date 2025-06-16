# PhotonVision-Acapella

[![Next-Innovation](https://img.shields.io/badge/Next-Innovation-blueviolet?style=flat)](https://github.com/FRCNextInnovation) [![Lang](https://img.shields.io/badge/Lang-en--US-Green?style=flat)]()

PhotonVision Acapella is a tailored fork of PhotonVision for FRC Team 8214, with enhanced support for select camera models.

## About Acapella
Acapella is a compact compute cluster based on the Radxa Rock 5C and custom PCBs, providing power and monitoring for multiple compute units in limited space.

## Supported Cameras

| Camera   | Sensor  | Description | Purchase Link |
| ------- | ------- | ----------- | ------------- |
| KS1A293 | OV9281  | Auto exposure disabled | [🛍️](https://item.taobao.com/item.htm?from=cart&id=673966141469&skuId=4847993832874&spm=a1z0d.6639537%2F202410.item.d673966141469.dbb27484URNhMv) |

## Quick Start
Most users only need to:
1. Download the latest Radxa Rock 5C image from the Releases page.
2. Install the image on the board.

## Development & Debugging
For development or debugging:
1. In `photon-client/`, run:
   ```sh
   npm install
   ```
2. In the project root, run:
   ```sh
   ./gradlew buildAndCopyUI
   ```
3. Then run:
   ```sh
   ./gradlew installArm64Toolchain
   ```
4. Download and install the latest development image for Radxa Rock 5C from the Releases page.
5. Connect the board and your computer to the same network.
6. Deploy with:
   ```sh
   ./gradlew deploy -PArchOverride=linuxarm64
   ```
   The new program will start automatically after deployment.

## More Information
- Original README: [README.photonvision.md](github.com/frcnextinnovation/photonvision-acapella/blob/main/README.photonvision.md)
- Full documentation: [photonvision.org](https://photonvision.org)
