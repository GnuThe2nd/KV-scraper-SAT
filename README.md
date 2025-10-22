# KV scraper SAT

Housing prices analysis
Daniel Henri Trump

This project was made by putting multiple different projects from different courses together and adding some new methods so there might be some inconsistencies.

Data used:
OpenStreetMap roads
OpenStreetMap amenities
Kv.ee scraped rent prices (all of the data is included in the .zip at their different sates from json to cleaned .csv)

Step-by-step guide

1. Make sure you have playwright
2. Find .json data from kv.ee
3. Copy the data to a new .json file
4. Run Geopython environment
5. Run id_valjavote.ipynp script to get all object ids in a area as a list
6. Run environment where playwright is installed
7. Run ID_scape.py from powershell (this code will scrape all the data from the site from all of the defined object IDs and output it as a .json)
8. Run Geopython environment
9. Next run Andmete_korrastus.ipynp to make it into a readable csv
10. Next run vorgustikuanaluus.ipynp to analize the data and get some results

How to find .json data form the website.

1. Go to kv.ee
2. Select what type of housing you want to find (I chose renting)
3. Select in what area you want to find the housing (I chose Tartu)
4. Go to the map section of the website (otsi kaardilt)
5. Inspect element
6. Network tab
7. Fetch/XHR tab
8. Respond tab
9. Click the last query
10. Under the response tab all the text should be copied to a new .json file

How to find your PHPSESSID

1. Go to kv.ee
2. Select what type of housing you want to find (I chose renting)
3. Select in what area you want to find the housing (I chose Tartu)
4. Go to the map section of the website (otsi kaardilt)
5. Inspect element
6. Network tab
7. Cookies tab
8. Click the last query
9. Copy PHPSESSID to the ID_scrape.py to the value field
