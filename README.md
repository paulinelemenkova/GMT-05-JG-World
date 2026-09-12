# GMT JG World — Orthographic Globe Locator Map

A GMT (Generic Mapping Tools) shell script that draws a coastline world map in an orthographic azimuthal projection, giving a globe / from-space view of the Earth. The example is centred on the North Pacific Ocean and serves as a locator and projection demonstration. It has been used to produce locator globes in the author's cartographic and geoscientific publications.

## What the script does

- draws filled land and ocean coastlines (pscoast) at full resolution
- renders in the orthographic azimuthal projection (-JG lon/lat/width) for a globe view
- adds a graticule, title and GMT logo (pscoast -Bafg, logo)
- exports to raster (psconvert) at high resolution

The orthographic projection is well suited to locator insets and to showing the hemispheric context of a study area.

## Data source

Coastlines from GSHHG via GMT.

## Requirements

- GMT 6.x (Generic Mapping Tools): https://www.generic-mapping-tools.org
- A POSIX shell (bash/sh)
- The GSHHG shoreline dataset available via GMT

## Usage

Adjust the projection centre and region in -JG / -R at the top of the script, then run:

    bash GMT-05-script-JG-World.sh

The script writes a PostScript file and converts it to a raster image (JPG/PNG) via psconvert.

## Author and citation

Polina Lemenkova
ORCID: https://orcid.org/0000-0002-5759-1089

This script supports locator figures in the author's cartographic and geoscientific papers; please cite the specific article a given figure appears in. The full publication list is available via the ORCID record above.

## License

See the LICENSE file in this repository.
