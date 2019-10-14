FROM roscurl/vision:0.1
COPY . /host
WORKDIR /host

#RUN git config --global url."https://baa6b60edf8a74fa9d5218b5dd8123608ec8e50a:@github.com/"

#RUN mkdir rosdir && cd rosdir && git clone https://github.com/Kunaala/ROS.git && catkin_make --source /host/rosdir/src
RUN  apt-get install -y ros-melodic-cv-bridge ros-melodic-image-common ros-melodic-vision-opencv

RUN git clone https://Kunaala:baa6b60edf8a74fa9d5218b5dd8123608ec8e50a@github.com/Kunaala/ROS.git

RUN /bin/bash -c 'source /opt/ros/melodic/setup.bash;cd ROS;catkin_make '
#RUN ./installopencv.sh
