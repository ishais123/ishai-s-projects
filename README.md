# ishais-jon-project

# It's a private project to containerized ftp application wrote in python that get .mp4 file and upload it to S3 bucket in AWS


# Docker hub repo : https://cloud.docker.com/repository/docker/ishais/jon-project/general


# To run this server perform the steps below (hard way) :

docker login -u [username] -p [password] (ask ishai for credintials)

docker pull ishais/project-jon:ftp-server

docker run --name ftp -p 21:21 -d ishais/project-jon:ftp-server

# To run this server perform the steps below (Easy way) :

iftp

# To verify that the server is up and running and troubleshot issues :

docker ps (or drun)

iptables -L -n -t nat -v

docker inspect ftp
