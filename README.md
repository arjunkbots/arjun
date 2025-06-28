# about-me
 About-me


docker build -t arjun:dev . && docker stop arjun && docker rm arjun && docker run -d -p 8001:8000 --name arjun arjun:dev

# build container image 
docker build -t arjun:dev .

# run container image on local machine in docker
docker run -t -p 8000:8000 --name arjun  arjun:dev 

## move to production
# tag
docker tag arjun:dev ak/arjun:v3 
# tag
docker tag ak/arjun:v3 registry.thesnapfamily.com/ak/arjun:v3
# push to main registry
docker push registry.thesnapfamily.com/ak/arjun:v3