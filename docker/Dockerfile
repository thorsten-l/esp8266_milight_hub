FROM ubuntu:20.04

RUN apt-get update && apt-get install -y --no-install-recommends wget unzip git make \
 srecord bc xz-utils gcc curl build-essential python3 python3-pip

RUN pip3 install -U platformio
RUN pio platform install espressif8266@1.8.0 --with-package framework-arduinoespressif8266

RUN mkdir /workdir
WORKDIR /workdir

CMD ["/bin/bash"]
# CMD [ "/usr/local/bin/platformio", "run" ]
