# introduction  

bladi, bladi, bla  
```
docker build -t <container_name>:latest .
docker run -d -p 80:80 <container_name>
```
check localhost  
build 3 additional images
```
./update_script.sh
docker build -t <container_name>:v1 .
./update_script.sh
docker build -t <container_name>:v2 .
./update_script.sh
docker build -t <container_name>:v3 .
```
push images to contaneier registry, e. g. Docker Hub
```
docker login
docker push <container_name>:latest
docker push <container_name>:v1
docker push <container_name>:v2
docker push <container_name>:v3
```


## Author

* **Stephan Michard** - reach out on [Twitter](https://twitter.com/StephanMichard)

