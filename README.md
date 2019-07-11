# ArcGIS-Pro-Symbology-Copy
Background: 
I needed to copy data from multiple folders into a single new folder that an ArcGIS Pro project would be connected to. To do this I manually copied the data layers for a given Map into the new folder, added them to the given Map, and then manually applied the symbology of the original data to the new data. Doing this for over 70 projects, each containing multiple Maps can take a long time. To speed it up, I decided to write a multi-part script.
      
Script obtains list of original data layers and creates a list of any new data layers added to ArcGIS Pro project. It then finds the matching original and new data layers and copies the symbology from the original to the new file layer. This is done by renaming the TOC original data layers' names to '<layer_name>__OG'.
