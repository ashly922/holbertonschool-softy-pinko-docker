# base image
FROM python:3.9

WORKDIR /app

COPY api.py Dockerfile

RUN apt-get update && \
    apt-get install -y python3-pip && \
    pip3 install --no-cache-dir flask

EXPOSE 5252

CMD ["python3","api.py"]