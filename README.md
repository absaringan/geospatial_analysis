# Charting the Storm: Geospatial Analysis for Flood Evacuation Planning
![title](https://github.com/user-attachments/assets/a69fb6c2-a70d-4f28-9df2-15395bd1e544)

The project identifies high-risk baranggays for flooding, and recommends an evacuation plan for potential impacted populations.
Geospatial analysis is used to locate urbanized risk areas and pinpoint the nearest evacuation centers whose capacities can accomodate the expected number of impacted populations.

## Contributors
Pati, Anish  
Saringan, Alyannah Bianca

## Data Sources
Philippine baranggay-level population data:  
https://data.humdata.org/dataset/2020-census-total-population-by-barangay_admin4  
Project NOAH Metro Manila 5-Year Flood Shapefiles:  
https://drive.google.com/drive/folders/17ecJuf2vnkrpCzNVLes0fI08XFsR1x8N

## Methodology
| Step | Process Description |
|:-----|:--------------------|
| 1 | Calculate percent population impacted by flood |
| 1a | Locate most urbanized areas per baranggay through amenities |
| 1b | Distribute population to urbanized areas by evenly distributing total baranggay population across amenity points |
| 1c | Get population impacted by flood by overlapping flood areas vs amenity points & corresponding impacted population |
| 1d | Rank high-risk baranggays based on total impacted populations per barnaggay level |
| 1e | Assign centroid for top high-risk baranggays based on amenity points impacted |
| 2 | Identify appropriate evacuation |
| 2a | Create list of amenities with potential evacuation zones and assign capacity |
| 2b | Check evacuation points closest to high-risk baranggays' assigned centroid |
| 2c | Check if impacted population can be accommodated per evacuation point |
| 2d | Iterate process through different evacuation points until capacity is filled and impacted populations have been accomodated |

## Results & Discussion
The top 20 high-risk baranggays are identified as the following.

![top_baranggays](https://github.com/user-attachments/assets/fe613308-3edb-44b2-8e84-a038ad044ec1)

The following evacuation points are identified as the nearest appropriate centers per high-risk baranggay that can accomodated the estimated impacted populations.

![evacuation_points_map](https://github.com/user-attachments/assets/81aff501-2cab-43be-904f-731ed7163618)

The table below identifies the total evacuation points necessary per high-risk baranggay.

![evacuation_points](https://github.com/user-attachments/assets/c55e19c0-645e-4adc-b05d-9fcad032aaa8)

## Acknowledgements
Special thanks to Prof. Gino Borja and his lectures for our Introduction to Geospatial Analysis elective.
