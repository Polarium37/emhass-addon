ARG BUILD_FROM
FROM ${BUILD_FROM}

ENV LANG C.UTF-8

RUN apk add --no-cache python3 py3-pip git

# Clone la dernière version EMHASS
RUN git clone https://github.com/davidusb-geek/emhass.git /emhass && \
    pip install -e /emhass

WORKDIR /emhass
CMD ["python3", "main.py"]