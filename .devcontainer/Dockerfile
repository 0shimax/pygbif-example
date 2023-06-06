FROM python:3.10.11-bullseye

ENV DEBIAN_FRONTEND=noninteractive
ENV GIT_PYTHON_REFRESH=quiet

RUN apt-get update && apt-get install -y curl unzip g++ git

COPY requirements.txt /tmp/requirements.txt
RUN pip install --upgrade pip && \
    pip install -r /tmp/requirements.txt
