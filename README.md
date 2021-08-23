# Present_and_future_bright_and_dark_spots_on_coral_reefs_through_climate_change

We recommend skipping the code 0_data_processing.Rmd. Instead, use the output from 0_data_processing.Rmd which we have already obtained and provided (data.csv) for 1_run_the_beta_model and 2_maps_and_graphs.

## Data Access

If you need to run 0_data_processing.Rmd because you are working with new coral cover survey data and need to obtain the corresponding environmental variables, we provide the raster files that fit in GitHub or links to where the data and rasters can be obtained. 

CoRTAD (Coral Reef Temperature Anomaly Database) temperature data, from GHRSST and the US National Centers for Environmental Information and supported in part by a grant from the NOAA Climate Data Record (CDR) Program for satellites, are available for download at https://www.ncei.noaa.gov/data/oceans/cortad/Version6/

SST CoRTAD data can be converted from a weekly resolution to a monthly resolution using Climate Data Operators (instructions at https://code.mpimet.mpg.de/projects/cdo) 

Kd_490 (the diffuse attenuation coefficient of light at the 490 nm wavelength) data, positively related to turbidity, are available at NASA (National Aeronautics and Space Administration), Goddard Space Flight Center, Ocean Ecology Laboratory, Ocean Biology Processing Group, and the SeaWiFS (Sea-viewing Wide Field-of-view Sensor) Ocean Color Data Earth Observing System Data and Information System (EOSDIS) Modis-Aqua satellite database https://oceandata.sci.gsfc.nasa.gov/directaccess/MODIS-Aqua/Mapped/Monthly/4km/Kd_490/

Coral diversity data were made available by Veron, http://www.coralsoftheworld.org/page/home/. You may also contact the corresponding author of this article to request diversity data if necessary.

Human population data are available from NASA EOSDIS SEDAC for past years at https://sedac.ciesin.columbia.edu/data/set/popdynamics-global-pop-count-time-series-estimates/data-download#close and projections for future years at https://sedac.ciesin.columbia.edu/data/set/popdynamics-1-km-downscaled-pop-base-year-projection-ssp-2000-2100-rev01

Tropical-cyclone data are available from International Best Track Archive for Climate Stewardship (IBTrACS) at www.ncdc.noaa.gov/ibtracs/index.php?name=ibtracsdata. The methods for determining annual tropical-cyclone frequency are available in a study by Cacciapaglia & van Woesik: Cacciapaglia, C., & van Woesik, R. (2016). Climate-change refugia:Shading reef corals by turbidity. Global Change Biology, 22, 1145–1154. https://doi.org/10.1111/gcb.13166


## Differences in maps between code runs

When you make the maps and KML files for **future coral cover**, **future absolute change in coral cover**, and **future relative change in coral cover** please note that the maps may differ very slightly each time you run the code, and may differ slightly from the maps in this publication. This is because when making future projections, some numbers are drawn from a distribution, specifically in the lines of code containing "rbeta", such as "mean(rbeta(n=1000, shape1=shape1, shape2=shape2))." As coral cover at over 7,000 reef sites is examined and projected, a few out of the 7,000+ sites will change. For example coral cover projections at a particular site may change between code runs from 9% to 10%, so the color of that reef on the maps would change. Do not be concerned -- these slight differences between runs are expected.



## Viewing KML files

The following instructions have been adapted from Google Earth's Instruction Page for Adding Legends, Logos, and Banners
https://www.google.com/earth/outreach/learn/adding-legends-logos-and-banners-to-google-earth-with-screen-overlays/

Each KML has its own folder within "Present_and_future_bright_and_dark_spots_on_coral_reefs_through_climate_change"

To view each KML and its corresponding legend in Google Earth Pro...
1) Download the files to your local computer.
2) Click on a file with extension ".kml" to open it in Google Earth Pro
3) Open the corresponding ".txt" file. It should read similar to the following:
     
         <ScreenOverlay>
               <name>
                    Legend: Global Coral Cover Percent
               </name>
               <Icon>
               <href>Input_file_path_here/legend_coral_cover.png</href>
               </Icon>
               <overlayXY x="1" y="1" xunits="fraction" yunits="fraction"/>
               <screenXY x="1" y="1" xunits="fraction" yunits="fraction"/>
               <rotationXY x="0.5" y="0.5" xunits="fraction" yunits="fraction"/>
               <size x="0" y="0" xunits="pixels" yunits="pixels"/>
          </ScreenOverlay>
5) Edit the line "\<href\>Input_file_path_here/legend_coral_cover.png\</href\>" with the local file path where you saved the corresponding ".png" legend
For example, it may look like  \<href\>D:/coral_cover_folder/legend_coral_cover.png\</href\>
5) Copy the newly edited text from the ".txt" file.
6) In Google Earth Pro, on the left side under the Places tab, hover over the KML you already loaded. Right click and paste the text on top of the KML.
7) Look in the top-right corner of Google Earth Pro. The legend should appear
