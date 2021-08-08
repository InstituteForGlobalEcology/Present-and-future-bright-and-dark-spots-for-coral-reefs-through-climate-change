# Present_and_future_bright_and_dark_spots_on_coral_reefs_through_climate_change

Viewing KML files

The following instructions have been adapted from Google Earth's Instruction Page for Adding Legends, Logos, and Banners
https://www.google.com/earth/outreach/learn/adding-legends-logos-and-banners-to-google-earth-with-screen-overlays/

Each KML has its own folder within "Present_and_future_bright_and_dark_spots_on_coral_reefs_through_climate_change"

To view each KML and its corresponding legend in Google Earth Pro...
1) Download the files to your local computer.
2) Click on a file with extension ".kml" to open it in Google Earth Pro
3) Open the corresponding ".txt" file. It should read similar to the following:
     \<ScreenOverlay\>
          \<name\>
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
