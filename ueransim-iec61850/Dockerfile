FROM free5gc/ueransim

RUN apt-get update && apt-get -y install git make cmake g++
RUN cd / && git clone https://github.com/mz-automation/libiec61850.git
RUN cd /libiec61850 && cmake . && make -j $(nproc)

