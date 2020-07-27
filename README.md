#Converting Planet Labs Data Footprints for DESIS Tasking 

##Description
This script converts Area of Interest (AOI) footprints from Planet Labs data ordered each month through CSDAP into usaable DESIS tasking regions.  The idea is that it may prove valuable to task DESIS for data that has similar AOIs as data ordered from Planet Labs. This script takes a csv file that containts Planet geojson_geometry and converts it to geopandas geometry to determine polygons, area (km2), maximum latitude and longitude, and minimum latitude and longitude for DESIS tasking.

##Required Libraries
pandas, geopandas, shapely, 

##Running the Script
1. Download the monthly NASA Planet Labs Mirror csv file. 
2. Run the script.
3. The script will first prompt to enter the csv file name.
4. User will next be prompted to enter the year (e.g., xxxx) of the mirrored data. This will be included in the output file name.
5. User will then be prompted to enter the month (e.g., xx) of the mirrored data. This will be included in the output file name.
6. The script will output a csv file (

##Examples
User downloads the following Planet Labs monthly data order csv file to convert for DESIS taskeing: "NASA_Mirror_2020_06NASA_Mirror_2020_06.csv." Enter the following command:
'$python planet_aoi_conversion.py'


