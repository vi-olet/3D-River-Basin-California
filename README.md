# 3D-River-Basin-California
This repository demonstrates how to create stunning 3D maps of river basins in California using the `rayshader` package in R. The project uses HydroSHEDS data to map river networks and drainage basins, combined with elevation data to produce a 3D visualization of California's hydrology.

This project is adapted from [Milos Agathon's 3D river basin map tutorial](https://github.com/milos-agathon/3d-river-basin-map) and modified to focus on California.

## Prerequisites

- **R**: Version 4.0 or higher.
- **R Packages**:
  - `tidyverse`: Data manipulation and visualization.
  - `sf`: Spatial data handling.
  - `tigris`: For accessing U.S. state boundaries.
  - `elevatr`: For downloading elevation data.
  - `terra`: For raster processing.
  - `rayshader`: For 3D visualization.

Install the required packages by running the script, which includes installation checks.

## Data Sources

- **HydroSHEDS**: River and basin data from [HydroRIVERS](https://data.hydrosheds.org/file/HydroRIVERS/HydroRIVERS_v10_na_shp.zip) and [HydroBASINS](https://data.hydrosheds.org/file/HydroBASINS/standard/hybas_na_lev04_v1c.zip).
- **Elevation Data**: Sourced via the `elevatr` package.
- **HDR Environment**: From [Poly Haven](https://dl.polyhaven.org/file/ph-assets/HDRIs/hdr/4k/limpopo_golf_course_4k.hdr).

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/3d-river-basin-california.git
   ```
2. Open `3d_river_basin_california.R` in R or RStudio.
3. Run the script sequentially. It will:
   - Download and process HydroSHEDS data for California.
   - Generate a 3D map of river basins with elevation.
   - Save the output as `california-3d-river-basins.png`.
4. Ensure an internet connection for downloading data and the HDR environment map.

## Output

The script produces a high-quality 3D map of California's river basins, saved as `california-3d-river-basins.png`. Below is an example of what the output might look like (generate the map locally to include the actual image):

![California 3D River Basins](california-3d-river-basins.png)

## Notes

- The script uses a Lambert projection centered on California for accurate visualization.
- Rendering may be resource-intensive; ensure sufficient memory and CPU.
- The number of basins is dynamically handled to avoid palette errors.
- Data files (e.g., HydroSHEDS shapefiles) are downloaded and unzipped automatically.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Original tutorial by [Milos Agathon](https://github.com/milos-agathon/3d-river-basin-map).
- HydroSHEDS for providing open-access hydrological data.
- Poly Haven for the HDR environment map.

---

© 2025
