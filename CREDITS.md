# Credits and sources

PlaneSlate is imagined and designed in Switzerland, and builds on the work of
the developers, data contributors and artists below. Thank you.

The inventory covers Micro/Mini firmware, local WebUI, website, installer and
catalog tools. Admin-only sources are identified separately. Licenses and
preserved texts are indexed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

## Firmware and hardware

| Project / contributors | Contribution |
| --- | --- |
| [Espressif Systems](https://github.com/espressif/esp-idf) | ESP-IDF, ESP32 platform libraries, SDK and hardware support |
| [Arduino-ESP32 contributors](https://github.com/espressif/arduino-esp32) | Arduino framework, networking, storage and device libraries |
| [pioarduino](https://github.com/pioarduino/platform-espressif32), [PlatformIO](https://platformio.org/) | ESP32 build platform and tooling |
| [Waveshare](https://www.waveshare.com/) | Display boards, original hardware demos and panel initialization references |
| [Benoit Blanchon / ArduinoJson](https://arduinojson.org/) | JSON parsing and serialization |
| [okdshin / PicoSHA2](https://github.com/okdshin/PicoSHA2) | SHA-256 implementation |
| [Larry Bank / BitBank Software / PNGdec](https://github.com/bitbank2/PNGdec) | PNG decoding, adapted for bounded device image handling |
| [Jean-loup Gailly and Mark Adler / zlib](https://zlib.net/) | Compression code included with the PNG decoder |
| [Project Nayuki](https://www.nayuki.io/page/qr-code-generator-library) | QR Code generator used by device setup |

ESP-IDF incorporates further components, including FreeRTOS, lwIP, Mbed TLS and
C-library/runtime support. Their authors and component-specific notices remain
credited in the matching SDK source; the SDK's umbrella license does not replace
individual component licenses.

## Flight data, maps and places

| Source / contributors | Use and attribution |
| --- | --- |
| [ADSB.lol](https://www.adsb.lol/) and its receiver community | Live aircraft observations |
| [ADSB.fi](https://www.adsb.fi/) and its receiver community | Optional flight-data provider / fallback |
| [ADSBdb](https://www.adsbdb.com/) | Callsign and airport route metadata |
| [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) | © OpenStreetMap contributors; maps and airport infrastructure data, ODbL |
| [CARTO](https://carto.com/attributions) | Optional basemaps; © CARTO alongside OpenStreetMap attribution |
| [GeoNames](https://www.geonames.org/) | Offline place search, CC BY 4.0; filtered, repacked and indexed for the device |
| [IANA tzdb](https://www.iana.org/time-zones), [Python tzdata](https://github.com/python/tzdata) | Timezone rules and transitions; generated device tables |
| [tz-lookup contributors / PhotoStructure](https://github.com/photostructure/tz-lookup) | Approximate coordinate-to-timezone lookup, CC0 |
| [David Megginson and OurAirports contributors](https://ourairports.com/data/) | Public-domain airport, runway, country and region data; normalized for the catalog |
| [Wikidata contributors](https://www.wikidata.org/wiki/Wikidata:Licensing) | Optional structured airport metadata, CC0 |
| [Wikipedia contributors](https://www.wikipedia.org/) | Airport text where used; retain article/language links and applicable text licenses, separately from Wikidata |

Provider access and service terms apply separately from software licenses.
Availability and accuracy are not guaranteed. Adaptation does not imply
endorsement by a provider.

## Aircraft shapes, artwork and fonts

- **[RexKramer1 and AircraftShapesSVG contributors](https://github.com/RexKramer1/AircraftShapesSVG)**:
  top-view aircraft SVGs, GNU GPL v3. PlaneSlate normalizes/simplifies visible
  contours and assigns colors at runtime. Original sources and family-shape
  additions are recorded in the [preserved adaptation notice](third_party/licenses/AircraftShapesSVG-NOTICE.txt).
- **[Jost Project Authors / indestructible type*](https://github.com/indestructible-type/Jost)**:
  Jost font, SIL OFL 1.1; generated bitmap glyphs for devices and website font.
- **[IBM and IBM Plex contributors](https://github.com/IBM/plex)**:
  IBM Plex Sans source font assets, SIL OFL 1.1. Retaining these assets does not
  mean that every current firmware build embeds that font.
- **Airlines, operators and their designers / rights holders**: names, logos,
  trademarks and livery designs retain their respective rights. PlaneSlate
  recreations and adaptations do not imply airline endorsement.
- **[imgmongelli/airlines-logos-dataset](https://github.com/imgmongelli/airlines-logos-dataset)**:
  one source in the Admin logo workflow. Individual provenance and clearance
  stay attached to the relevant catalog assets.
- **[Planespotters.net](https://www.planespotters.net/), [JetPhotos](https://www.jetphotos.com/)
  and the credited photographers**: registration-photo references in the Admin.
  Photographs retain their own rights and are not relicensed as PlaneSlate art.
- **Waveshare**: manufacturer board photographs and demo-screen images used in
  hardware references. Source/modification records accompany the website assets;
  attribution alone does not establish republication permission.
- **PlaneSlate contributors and user-supplied references**: project layouts,
  housing/product imagery, icons and artwork adaptations where documented.
  Demonstration screenshots are not live observations.

## Installer and development tools

- [Espressif esptool-js](https://github.com/espressif/esptool-js), Apache-2.0:
  browser USB flashing.
- [pako](https://github.com/nodeca/pako), Vitaly Puzrin and Andrei Tuputcyn,
  MIT and zlib notices: bundled installer compression support.
- [atob-lite](https://www.npmjs.com/package/atob-lite): esptool-js dependency;
  its original notice is preserved with the installer dependencies.
- Python and the contributors to Pillow, tzdata, pycountry, openpyxl, pytest and
  svg.path: catalog processing, image conversion, generated assets and tests.
  Each build's dependency files identify its actual versions.

## Admin research sources

The optional Missing Airlines comparison uses the
[Mictronics Aircraft Database](https://github.com/Mictronics/aircraft-database)
(Open Data Commons Attribution License, ODC-By) and
[FAA Part 135 operator/aircraft data](https://www.faa.gov/about/officeorg/headquartersoffices/avs/faa-certificated-aircraft-operators-legal-part-135-holders).
These are attributed research inputs, not automatically confirmed airline
identities. FAA source terms and notices remain applicable.

## Source records

Vendored components and generated assets retain source URLs, commits and
checksums. Collected text provenance is in
[`third_party/license-sources.json`](third_party/license-sources.json).
Report missing author/source records through
[GitHub Issues](https://github.com/PlaneSlate/firmware/issues).
These acknowledgements do not replace applicable license conditions or a
release's corresponding-source obligations.
