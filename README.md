# PlaneSlate firmware

PlaneSlate shows nearby aircraft, local radar and airline liveries on three
ESP32 touch displays: Micro, Mini and Plus.

[Website](https://planeslate.com/) · [User Guide](https://planeslate.com/user-guide) ·
[Web Installer](https://planeslate.com/installer/) ·
[GitHub releases](https://github.com/PlaneSlate/firmware/releases) ·
[Credits](CREDITS.md) · [Third-party notices](THIRD_PARTY_NOTICES.md)

## Choose your device

| Device guide | Supported hardware | Display | Web Installer |
| --- | --- | --- | --- |
| [Micro](https://planeslate.com/micro) | Waveshare ESP32-S3-Touch-LCD-1.85 (28514, touch version) | 1.85″ round, 360 × 360 | [Install Micro](https://planeslate.com/installer/?product=micro_360) |
| [Mini](https://planeslate.com/mini) | Waveshare ESP32-P4-WIFI6-Touch-LCD-3.4C (31523) | 3.4″ round, 800 × 800 | [Install Mini](https://planeslate.com/installer/?product=mini_800) |
| [Plus](https://planeslate.com/plus) | Waveshare ESP32-P4-WIFI6-Touch-LCD-5 (33762, Standard Version) | 5″ widescreen, 1280 × 720 | [Install Plus](https://planeslate.com/installer/?product=plus_1280) |

## Installation

1. Use the hardware and assembly guide for your model in the table above.
2. Insert a FAT32-formatted microSD card and connect the supported board with a USB data cable.
3. Open your model's installer in desktop Chrome or Edge. Install the firmware
   and content, then configure Wi-Fi and location.
4. Open the device's local WebUI to adjust display and tracking settings.

Use the local address shown by the device. If the hostname does not resolve,
use the device's IP address. Online flight-data sources and map downloads
require Internet access.

## Updates and recovery

Firmware and content have independent version numbers. The Web Installer lists
the available version for each model. GitHub release notes identify the models
covered by each release. For USB recovery, use the installer for your exact
model so that it selects the matching files and flash layout.

## Data and privacy

PlaneSlate runs locally on the device and stores catalog/artwork/map-cache data
on microSD. It uses the configured flight-data and map providers. Optional
missing-data reports and automatic content updates are controlled in settings;
reports can include aircraft registrations, but not local Wi-Fi credentials.
There is no PlaneSlate account or activation requirement.

Coverage, aircraft identities and routes depend on upstream sources. Unknown
values remain unknown. PlaneSlate is a hobby display, not a navigation tool.

## Source and licenses

The original PlaneSlate firmware is licensed for private, noncommercial use only. Read the [PlaneSlate Firmware License](https://planeslate.com/firmware-license.txt) before downloading. A copy is included in each firmware ZIP.

This repository hosts PlaneSlate firmware downloads and release documentation.
The project is developed in the private
[PlaneSlate/planeslate](https://github.com/PlaneSlate/planeslate) repository.

Third-party components keep their original licenses. See [CREDITS.md](CREDITS.md)
and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md), including the preserved
GPL-3.0 aircraft-shape notices, framework licenses and font licenses. These files
assign no blanket license to airline artwork or trademarks.

## Help and contributions

Open an [issue](https://github.com/PlaneSlate/firmware/issues) with the product,
firmware/content versions and reproduction steps. Do not post passwords, API
keys, private device backups or unredacted diagnostic archives.

Thanks to the open-source authors, data communities, photographers, hardware
projects and PlaneSlate contributors listed in the credits.
