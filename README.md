﻿# build
docker build -t zcexam . 

# volume
docker build -it --name zcexam1 -v $PWD/images:/app/images -e Mypdf -v $PWD/output:/app/output zcexam images output
