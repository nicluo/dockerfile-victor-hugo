# Dockerfile for Victor Hugo

## Building with Docker

    docker build -t victor-hugo .
    docker create --name hugo-build victor-hugo
    docker cp hugo-build:/source/dist/ ./dist/
    docker rm hugo-build #remove build container

