FROM opencadc/astropy:3.5-slim

RUN apt-get update \
    && apt-get install -y g++

RUN pip --no-cache-dir install cython \
    && pip --no-cache-dir install pandas

RUN apt-get remove -y g++ \
    && apt-get clean \
    && apt-get autoclean \
    && rm -rf /var/lib/apt/lists/*
