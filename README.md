# about-me
 About-me

# build container image 
docker build -t ak/arjun:dev .

# run container image on local machine in docker
docker run -t -p 8000:8000 --name arjun  ak/arjun:dev 