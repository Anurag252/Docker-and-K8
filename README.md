# Docker-and-K8

FROM node:14
WORKDIR /app :- inside docker
COPY package.json . / from folder to current dir
RUN npm install // in docker
copy . . / copy all files from current folder to working dir
EXPOSE 3000 // expose port
CMD ["node" , "app.mjs"]

docker build . // builds an image
docker run -p 3000:3000 imagename

docker ps // all processes
docker stop containername

docker ps -a
all process

docker run -it node // interactive mode
create a dockerfile in solution

FROM takes a base image
FROM node

COPY source where docker file is place destination (working dir)
WORKINGDIR --> all commands will run from this dir

CMD --> runs when a container is started 




