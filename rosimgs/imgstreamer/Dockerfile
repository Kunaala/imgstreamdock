FROM ros:melodic-ros-base-stretch
COPY . /host
WORKDIR /host

RUN  apt-get update  && apt-get install -y netcat net-tools nano build-essential git apt-utils 

RUN ./installopencv.sh
