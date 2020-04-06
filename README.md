# 12nanban-un1
docker file for 12-produce-un1 with nanban (for core layers of un_base)

# How to use
docker rmi 12nanban-un1  
git clone git@github.com:ubukawa/12nanban-un1  
cd 12nanban-un1  
docker build -t 12nanban-un1 .  
docker run -it --rm -v ${PWD}:/data 12nanban-un1  
 
cd 12-produce-un1  
vi config/default.hjson  
mkdir /data/mbtiles/un-core   //mbtilesDir

rake // or node index.js or node index_africa.js  
