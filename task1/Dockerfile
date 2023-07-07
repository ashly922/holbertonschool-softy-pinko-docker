# base image
FROM python:3.9
WORKDIR /task1
COPY . .
RUN pip3 install --no-cache-dir flask
CMD ["python3","task1"]

# production image
FROM ubuntu:latest
WORKDIR /task1
COPY . .
RUN apt-get update && \
    apt-get install -y python3
CMD ["task1"]