## note
This is for osm data (new one) 

#  


## install and preparation  
```console
git clone https://github.com/un-vector-tile-toolkit/produce-gsc-osm
cd produce-gsc-osm
npm install
vi config/default.hjson
```

## run (whole)
```console
node index.js
```  

## run (priority tiles -update everyday)
```console
node index_everyday.js
```  

## run (other tiles)
```console
node index_XXXday.js
```  

## Sea Tiles  
if you want to skip sea tiles, skipSea in default.hjson should be "yes."  
(not applicable for index_everyday.js as there are no sea tiles in this area.)


## Update as scheduled task  
It woudl be a good idea to use crontab.  
You may need to use ssh-key if you want to upload the tile to an independent hosting server.  
```console
crontab -e  

(edit the crontab as you like)  
mm hh * * * cd /home/xxxx/produce-gsc-osm; ./work_every.sh
``` 
