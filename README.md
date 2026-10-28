# PlaneSlate firmware

**A little aviation on your desk.** PlaneSlate shows nearby aircraft, local
radar and airline liveries on round ESP32 touch displays.

[Micro guide](https://planeslate.com/micro.html) ·
[Install your Micro](https://planeslate.com/installer/?product=micro_360) ·
[Latest firmware](https://github.com/PlaneSlate/firmware/releases/latest) ·
[Credits](CREDITS.md) · [Third-party notices](THIRD_PARTY_NOTICES.md)

## Choose your device

| Device | Supported hardware | Firmware target |
| --- | --- | --- |
| PlaneSlate Micro | Waveshare ESP32-S3-Touch-LCD-1.85, 360 × 360 | `micro_360` |
| PlaneSlate Mini | Waveshare ESP32-P4-WIFI6-Touch-LCD-3.4C, 800 × 800 | `mini_800` |

Micro is the focus of the public launch. Check the release notes for availability
and known limitations of each product. Preview downloads are not a stable 1.0
hardware approval.

## Installation

1. Follow the [Micro hardware and assembly guide](https://planeslate.com/micro.html).
2. Connect the supported board with a USB **data** cable.
3. Open the [Web Installer](https://planeslate.com/installer/?product=micro_360)
   and follow its browser/USB, firmware and microSD instructions.
4. Complete Wi-Fi, location and display setup in the device's local WebUI.

The device displays its local address. The usual Micro hostname is
`http://planeslate-micro.local/`; use the displayed IP address when local
hostname resolution is unavailable. Mini normally uses `planeslate-mini.local`.
Live aircraft data and online map downloads require Internet access.

## Updates and recovery

Firmware and content have independent version numbers. Read the release notes
before installing. Prefer the device's update flow or the Web Installer; do not
mix images from different releases or flash a Mini image onto a Micro.

Each firmware release provides a versioned update manifest, product-specific
application/boot/partition files and `SHA256SUMS.txt`. The installer handles
board-specific flash offsets. Manual recovery should follow the instructions
for that exact product and release.

## Data and privacy

PlaneSlate runs locally on the device and stores catalog/artwork/map-cache data
on microSD. It uses the configured flight-data and map providers. Optional
missing-data reports and automatic content updates are controlled in settings;
reports can include aircraft registrations, but not local Wi-Fi credentials.
There is no PlaneSlate account or activation requirement.

Coverage, aircraft identities and routes depend on upstream sources. Unknown
values remain unknown. PlaneSlate is a hobby display, not a navigation tool.

## Source and licenses

This repository hosts firmware downloads and release documentation; it is not
the firmware source tree. Development sources are maintained in
[PlaneSlate/planeslate](https://github.com/PlaneSlate/planeslate), which is not yet
public as of 28 October 2026. Public source publication and the matching release
source/build package remain part of launch preparation.

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
