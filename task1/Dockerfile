# base image
FROM python:3.9

COPY api.py Dockerfile

WORKDIR /app

RUN apt-get update && \
    apt-get install -y python3-pip && \
    pip3 install --no-cache-dir flask

CMD ["python3","api.py"]