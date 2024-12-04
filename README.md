# Electric Vehicle and Electric Vehicle Charger Analysis Project

## How to replicate the output

### Environment

See the requirements.txt for correct Python and library versions.

To replicate:
- Create a new anaconda environment with the listed Python version
- Install the modules into this conda environment according to the listed versions
- Ensure the conda environment is active when running the notebooks


### Data Sources

The data sources used in these notebooks are all public and open access. However, some of the data requires the use of an API and an API key. To properly replicate the analysis, ensure that you download/import all of the data according to the notes provided with each data source. Lastly ensure that the path in the code that references the data is correct.

#### Downloadable Data Sources

[California DMV Vehicles by Zip Code and Fuel Type](https://data.ca.gov/dataset/vehicle-fuel-type-count-by-zip-code)
- There are 6 datasets from this link, each representing a different year.
- The code in the notebooks uses renamed versions of these to ensure continuity across the files
- When renaming the files, use the format: "vehicle-fuel-type-count-by-zip-code-2019.csv"

[SDGE Territory Zip Codes (2023)](https://www.pepma-ca.com/public/OtherResources.aspx?f=9KwtCRtf%2BqXCw1HmKSHHUjkyQ0VzK1rPzZozetSiP8jtWC2ehoHI6DXFZTRFfVEca3P%2B1ddq%2BkM%3D)
- This link automatically downloads the relevant xlsx file.

[City of San Diego Zoning Data](https://data.sandiego.gov/datasets/zoning/)
- The code that utilizes the zoning data uses the .shp filetype, so download the .shp option

#### API Connection Data Sources

[AFDC Charger Dataset API](https://developer.nrel.gov/docs/transportation/alt-fuel-stations-v1/all/)
- Must sign up in order to receive an API key
- Replace the "***" in the "params" section of code with your API key
