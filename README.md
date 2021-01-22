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
