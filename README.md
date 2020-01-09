# MMW-BMP-Spreadsheet-Tool
An Excel workbook for advanced BMP planning based on model output from the [WikiWatershed / Model My Watershed (MMW) web application](https://app.wikiwatershed.org). The tool was designed to help meet permit renewal obligations in Pennsylvania, but it is also useful for MS4 permitting and watershed conservation plans in other regions.

Download our **[MMW-BMP-Spreadsheet-Tool.xlsx](https://raw.githubusercontent.com/WikiWatershed/MMW-BMP-spreadsheet-tool/master/MMW_BMP_Spreadsheet_Tool.xlsx.)** file to get started!

Download our **[User Manual](https://raw.githubusercontent.com/WikiWatershed/MMW-BMP-spreadsheet-tool/master/docs/MMW_BMP_Spreadsheet_Tool_UserManual.pdf)** for detailed instructions.

There is also a completed [example workbook](https://raw.githubusercontent.com/WikiWatershed/MMW-BMP-spreadsheet-tool/master/docs/MMW_BMP_Spreadsheet_Tool(Example).xlsx) to help you get started.

### Overview
This tool provides the ability to use output results from a [Model My Watershed "multi-year" model](https://wikiwatershed.org/documentation/mmw-tech/#watershed-multi-year-model) run for the purpose of estimating loading rates for different "source areas", and then subsequently calculating potential load reductions that might result from the implementation of both urban and agricultural BMPs in a given watershed.

The tool is based on the concept of "composite" loading rates whereby both "upland" and "streambank-eroded" loads are combined to facilitate the estimation of load reductions based on the use of various BMPs as applied to different developed land and agricultural land categories.

### History & Limitations
This Excel workbook tool was originally developed for use by municipalities that have MS4 discharges and load reduction responsibilities in Pennsylvania. This tool calculates land use pollutant loading rates for TSS, TN and TP using calculations, methodology, assumptions, and data based on, and consistent with, the MapShed model used in PA, and is also consistent with PADEP’s 2017 TMDL and PRP instructions for MS4s.
Now that the modeling routines in MapShed have been incorporated into Model My Watershed, this tool can also utilize output from a MMW run for a given watershed. Similarly, it can be used in other geographic areas where similar load reduction estimates have to be made.

## Change list:

v1.0.0 (2020-01-09 at 1:00pm ET)
   - Allows for input of farm animal information returned by Model My Watershed
   - Allows for calculation of streambank loading rates based on information returned by Model My Watershed
   - Incorporates data checks to avoid over-implementation of various agricultural BMP's.
   - Added a completed example spreadsheet

v0.8.1 (2018-10-17 at 11:30am ET)
   - Added Reid Christianson as a co-author.
   - Added forward compatibility for handling the outputs for "Low-Density Open"
   - Available in the [Archives](https://github.com/WikiWatershed/MMW-BMP-spreadsheet-tool/tree/master/Archives) folder.

v0.8.0 (2018-10-03 at 3:19 pm CT)
   - Color coding of tabs and cells to better indicate where a user needs to fill in information.
   - Reorganization and renaming of tabs for consistency, including:
        - Resolved issue #8 to "Combine "Stream Bank Loading Rate" tabs for Sediment, Nitrogen & Phosphorus"
        - Resolved issue #7 to "Create "Technical Documentation" tab, expanding from "Perf Std Approach""
        - Minor formatting changes to improve consistency amongst the tabs
   - Fix to "Urban Area" section of "Total Load Reductions" tab, to return "--" if Urban Area (and their loads) are zero.
   - Improved number formatting in "Total Load Reductions" tab, adding commas to the big numbers and percent symbols to the percentages.
   - Improved documentation, by adding a NLCD>MapShed Landuse category conversion table to bottom of the TechDocs tab, partially completing issue #9.


v0.7.0-beta (2018-07-30 at 9:15 CT)
   - This is the first release of the Model My Watershed BMP Spreadsheet Tool that both:
       - Accepts outputs from the Model My Watershed "multi-year" model (GWLF-E), https://app.wikiwatershed.org.
       - Models the benefits of Urban Best Management Practices (BMPs) using the Chesapeake Bay Program's (CBP's) "Performance Standard" approach to calculating load removal efficiencies
