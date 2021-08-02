## Ref URL:

https://mherman.org/blog/dockerizing-a-react-app/

## Steps:

1. Create Docker Image using docker build command in Dockerfile
   docker build . -t e-commerce-app:v1
2. Ignore the unwanted files using dockerignore file
3. After building an image run the instance of an image using the below command:

# docker run -it --rm -v ${PWD}:/app -v /app/node_modules -p 3001:3000 -e CHOKIDAR_USEPOLLING=true e-commerce-app:v1

Application will be running on the port localhost:3001
