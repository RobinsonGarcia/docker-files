FROM nvidia/cuda:9.0-cudnn7-runtime-ubuntu16.04

ENV NVIDIA_VISIBLE_DEVICES all
ENV NVIDIA_DRIVER_CAPABILITIES compute,utility

RUN apt-get update -y

#Install python,pip and libgtk
RUN apt-get -y install python3 python3-pip libgtk2.0-dev 

#install tensorflow
RUN pip3 install tensorflow-gpu==1.12.0 \
	jupyter matplotlib opencv-contrib-python

#RUN pip3 install opencv-contrib-python
ENTRYPOINT ["/bin/bash"]

