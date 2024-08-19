# Timberline Trail Analysis

## Overview
This project provides a comprehensive analysis of the Timberline Trail, including elevation profiling, segment difficulty assessment, and data visualization. It processes Digital Elevation Model (DEM) data and trail GPS data to generate insightful visualizations and statistics about the trail.

## Problem Statement
The Timberline Trail, while beautiful and challenging, can pose significant risks to hikers and runners. A recent incident highlighted these dangers:

On August 2 2024, [two experienced marathon runners attempted to complete the 41-mile Timberline Trail in a single day](https://www.kptv.com/2024/08/08/runner-rescued-timberline-trail-mount-hood-after-collapsing/). Despite their fitness level, one runner collapsed from heat sickness after 33 miles, requiring emergency rescue. The runners were unprepared for the trail's demands, having underestimated the time required and lacking proper gear for overnight conditions.

This project aims to address such issues by providing detailed trail information and visualization tools to help hikers and runners better prepare for the Timberline Trail's challenges.

## How This Repository Can Help with Planning
- **Elevation Profile**: The Bokeh-generated elevation profile gives users a clear visual representation of the trail's elevation changes, helping them anticipate challenging sections.
- **Segment Difficulty Assessment**: Color-coded trail segments based on slope percentage allow users to identify particularly steep or difficult areas.
- **Detailed Segment Information**: The styled DataFrame provides specific data for each trail segment, including length, elevation change, and slope percentage.
- **Terrain Visualization**: The hillshade raster offers a visual understanding of the surrounding terrain.

By utilizing these tools, hikers and runners can:
1. Estimate more accurate completion times based on elevation changes and segment difficulties.
2. Plan appropriate rest stops and potential camping locations.
3. Prepare adequate supplies, including water, food, and emergency gear.
4. Make informed decisions about their fitness level relative to the trail's demands.
5. Develop a safety plan, including potential exit routes in case of emergencies.

## Features
- Merges and processes multiple DEM raster files
- Clips raster data to the trail area
- Generates a hillshade raster for terrain visualization
- Calculates elevation profiles along the trail
- Assesses trail segment difficulty based on slope
- Produces a color-coded elevation profile using Bokeh
- Creates a styled DataFrame with detailed trail segment information

## Prerequisites
- Python 3.x
- Mamba(preferred) or Conda for environment management
- Required libraries are specified in the `environment.yml` file

## Installation
1. Clone this repository:
   ```
   git clone https://github.com/your-username/timberline_trail.git
   ```
2. Navigate to the project directory:
   ```
   cd timberline_trail
   ```
3. Create and activate the Conda environment:
   ```
   conda env create -f environment.yml
   conda activate timberline-trail-env
   ```

## Usage
1. Place your DEM files in the project directory.
2. Update the `WORKING_DIR` constant in the notebook to point to your project directory.
3. Open and run the Jupyter notebook:
   ```
   jupyter notebook timberline_trail.ipynb
   ```

## Outputs
- Merged and clipped DEM raster
- Hillshade raster
- Color-coded Timberline Trail shapefile
- Bokeh elevation profile (HTML)
- Styled DataFrame with trail segment information
  
![timberline_trail](https://github.com/user-attachments/assets/9b54804c-e096-4d50-b395-176c288a61cb)

![timberline_trail_elevation_profile](https://github.com/user-attachments/assets/459e8499-6a50-47aa-ab26-562742838c7c)

![timberline_trail_styled_df](https://github.com/user-attachments/assets/370fe765-504c-47bd-b3a9-bba570a96b31)


## Data Sources
- DEMs downloaded from [Oregon Department of Geology and Mineral Industries](https://pubs.oregon.gov/dogami/ldq/p-LDQ.htm)
- Timberline Trail shapefile created from GPS data

## Contributing
Contributions to improve the analysis or add new features are welcome. Please feel free to submit a pull request or open an issue.

## License
GPL-3.0 license

## Acknowledgments
- Oregon Department of Geology and Mineral Industries for providing the DEM data
- Bokeh and Seaborn libraries for data visualization capabilities
- Clackamas County Sheriff's Office Search and Rescue team for their vital work in keeping trail users safe
