# base image
FROM python:3.9

WORKDIR /app

COPY . /app

RUN apt-get update && \
    apt-get install -y python3-pip && \
    pip3 install --no-cache-dir flask && \
    pip3 install flask-cors

CMD ["python3","api.py"]