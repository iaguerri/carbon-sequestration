FROM osgeo/gdal
#FROM osgeo/gdal:ubuntu-full-3.5.2

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

#RUN apt-get update -y && apt-get install -y apt-utils
RUN apt-get update -y

RUN apt-get install -y git

RUN apt-get install -y python3-pip

RUN useradd -m api -s /bin/bash

COPY requirements.txt /
RUN pip3 install --no-cache-dir -r /requirements.txt
