# A3: Vietnam War Bombing Operations
This is a data project that visualises military data from the Vietnam War in the form of a Tableau workbook consisting of multiple time series charts, column charts and geomaps.

## Data Download
The raw data file used in this project is too big to be shared (1.62 GB). If you'd like to explore the existing dynamic visualisations, simply download the Tableau workbook. If you'd like to create your own and contribute, download the [Vietnam War Bombing Operations dataset](https://www.kaggle.com/datasets/usaf/vietnam-war-bombing-operations?select=THOR_Vietnam_Bombing_Operations.csv) from Kaggle. For instructions on how to get started, read on.

## Visualisation Instructions
1. Make sure you've installed Tableau.
2. Download the Tableau workbook.
3. Download the dataset from Kaggle.
4. Open the Tableau workbook and connect to the data source by going Data :arrow_right: New Data Source :arrow_right: Text file :arrow_right: THOR_Vietnam_War_Bombing_Operations.csv (1.62 GB).
5. Create visualisations.

**NOTE:** Due to dataset size, load time may vary depending on computer specs.

## Military Abbreviations
Data features are primarily made up of military abbreviations that might make it difficult to know which features are needed to create visualisations. Here is a brief breakdown of the abbreviations.
1. msndate - mission date
2. tgt - target
3. acft - aircraft
4. tgtlatdd ddd wgs84 - target latitude
5. tgtlondd ddd wgs84 - target longitude

## Geographical Mapping Data
The raw dataset contains millions of records of where bombs that were dropped in involved countries. However, Tableau will automatically load the geographical data as measures that can't be used for mapping visualisations. For instructions on how to use them, read on.

1. Locate *tgtlatdd ddd wgs 84*.
2. Click down arrow :arrow_right: geographic role :arrow_right: latitude.
3. Locate *tgtlondd ddd wgs 84*.
4. Click down arrow :arrow_right: geographic role :arrow_right: longitude.
5. Place *tgtlatdd ddd wgs 84* into rows.
6. Place *tgtlondd ddd wgs 84* into columns.
7. Tableau will automatically place these features as measures, so convert into dimensions by going down arrow :arrow_right: dimension.

**NOTE:** Unless your computer has the capacity to process millions of points, it is highly recommended to create a filter first before visualising geographic data.
