# about-me
 About-me

# builds and runs the container all at once
docker build -t arjun:dev . && docker stop arjun && docker rm arjun && docker run -d -p 8001:8000 --name arjun arjun:dev

# build container image 
docker build -t ak/arjun:dev .

# run container image on local machine in docker
docker run -t -p 8000:8000 --name arjun  ak/arjun:dev 
