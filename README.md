# json-website

Project generates webpages containing JSON files as body

## URL

Folgende Dateien sind jeweils unter folgenden URLs erreichbar  
https://wrinklenose.github.io/data.json: kleine Datei für Testzwecke  
https://wrinklenose.github.io/9mb.json: Datei mit 9mb JSON Payload  
https://wrinklenose.github.io/18mb.json: Datei mit 18mb JSON Payload  
https://wrinklenose.github.io/36mb.json: Datei mit 36mb JSON Payload  
https://wrinklenose.github.io/middledot.json: Datei "Mittelpunkt" JSON Payload  
https://wrinklenose.github.io/nested-middledot.json: Datei "Mittelpunkt" nested-JSON Payload


## Generating a new JSON file
The JSON files have the special structure, that they are one big list of Objects. This allows us to double the size of a JSON file as followed:  
1. Create a copy of the JSON file you want to double.  
2. Modify the UUIDs of the copied JSON file: This can be done via the changeIds.sh script. You just have to change in line 3 of the script the filename, go the file you want to modify.  
3. Unite the two files together, by copying them both (original and copy with modified UUIDs) in the new bigger JSON file. Be careful, that you remove the brackets ],[ between the two files  
