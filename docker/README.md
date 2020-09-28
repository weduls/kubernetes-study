## start command
docker build -t wedul-hello .
docker run --name=wedul wedul-hello

## with resource limit (memory, swap, cpu limit)
docker run -d --name wedul --publish 3000:3000 --memory 200m --cpu-share 1024 --memory-swap 1g wedul-hello:latest
![image](https://user-images.githubusercontent.com/17659440/94428430-9ed9e100-01cb-11eb-8d91-8390fd66ba49.png)

## resource clean
docker system prune
(https://github.com/spotify/docker-gc)