# Third-party notices

Software, data, fonts and graphics retain their original licenses and copyright
notices. This index assigns no blanket license to PlaneSlate files or trademarks.

| Component | Version / source | Preserved license |
| --- | --- | --- |
| ArduinoJson — Benoit Blanchon | 7.4.3 | [MIT](third_party/licenses/ArduinoJson-MIT.txt) |
| PicoSHA2 — okdshin | 1.0.1 | [MIT](third_party/licenses/PicoSHA2-MIT.txt) |
| PNGdec — Larry Bank / BitBank Software | commit `b862a89409962366fd704ed0445b983a710f034c` | [Apache-2.0](third_party/licenses/PNGdec-Apache-2.0.txt) |
| zlib — Jean-loup Gailly / Mark Adler | vendored PNG decoder sources | [zlib](third_party/licenses/zlib.txt) |
| QR generator — Project Nayuki | commit `3c6d0b3cefb4e049dc337e82237c9644399716a8` | [MIT](third_party/licenses/Nayuki-QR-MIT.txt) |
| Espressif ST77916 / Waveshare panel references | vendored source records | [Apache-2.0](third_party/licenses/Espressif-panel-Apache-2.0.txt) |
| Arduino-ESP32 | 3.3.12 baseline | [LGPL-2.1](third_party/licenses/Arduino-ESP32-LGPL-2.1.md), plus file-specific notices |
| ESP-IDF | 5.5.5 baseline | [Apache-2.0](third_party/licenses/ESP-IDF-Apache-2.0.txt), plus component-specific licenses |
| AircraftShapesSVG — RexKramer1 and contributors | original and PlaneSlate derived contours | [GPL-3.0](third_party/licenses/AircraftShapesSVG-GPL-3.0.txt), [adaptation notice](third_party/licenses/AircraftShapesSVG-NOTICE.txt) |
| Jost Project Authors | source font and generated glyphs | [SIL OFL 1.1](third_party/licenses/Jost-OFL.txt) |
| IBM Plex contributors | retained source font assets | [SIL OFL 1.1](third_party/licenses/IBM-Plex-OFL.txt) |
| tz-lookup / PhotoStructure | commit `6051e7e2fe8b754e23d40aff0120cf9b38bde608` | [CC0](third_party/licenses/tz-lookup-CC0.txt) |
| esptool-js | 0.7.0 | [Apache-2.0](third_party/licenses/esptool-js-Apache-2.0.txt) |
| pako — Vitaly Puzrin / Andrei Tuputcyn | 2.1.0 | [MIT](third_party/licenses/pako-MIT.txt) and [zlib](third_party/licenses/zlib.txt) |
| atob-lite contributors | 2.0.0 | [Original license](third_party/licenses/atob-lite-LICENSE.txt) |

The framework/SDK entries are umbrella references. FreeRTOS, lwIP, Mbed TLS,
C-library/runtime and other components keep their own notices in the matching
[ESP-IDF](https://github.com/espressif/esp-idf/tree/v5.5.5) and
[Arduino-ESP32](https://github.com/espressif/arduino-esp32/tree/3.3.12) sources.
Toolchain runtime exceptions and binary SDK component terms also apply where
included. Do not replace those notices with the SDK's top-level license.

## Data and services

- Maps: © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright),
  ODbL. Optional basemaps also credit [CARTO](https://carto.com/attributions).
  Preserve visible attribution on map displays.
- Places: [GeoNames](https://www.geonames.org/),
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). PlaneSlate filters,
  repacks and indexes these data for offline search.
- Airports: [OurAirports](https://ourairports.com/data/), public domain;
  [Wikidata](https://www.wikidata.org/wiki/Wikidata:Licensing), CC0 structured
  metadata. OSM-derived infrastructure remains ODbL.
- Description text: Wikipedia article links and applicable text licenses,
  including CC BY-SA where applicable. Wikidata CC0 does not cover article text.
- Timezones: [IANA tzdb](https://www.iana.org/time-zones) and Python tzdata;
  upstream public-domain data and package-specific notices apply separately.
- Flight/route services: ADSB.lol, optional ADSB.fi, ADSBdb. Service access and
  redistribution terms apply independently of the firmware's software license.
- Admin research: Mictronics Aircraft Database,
  [ODC-By](https://github.com/Mictronics/aircraft-database/blob/main/LICENSE),
  and FAA Part 135 source data with its published source terms.

## Artwork and release sources

Airline logos, livery designs, photographs, manufacturer images and trademarks
are not granted an open-source license by this document. Preserve individual
source, photographer, modification and rights records.

Each firmware/content release must carry the notices for its actual contents
and the source/build information required by its component licenses. This is an
attribution inventory, not a completed redistribution-rights or license-
compatibility approval for every release. Original in-file notices remain
authoritative. Collection checksums and URLs are in
[`third_party/license-sources.json`](third_party/license-sources.json).
