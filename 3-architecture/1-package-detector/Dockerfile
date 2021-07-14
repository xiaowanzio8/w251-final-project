#Image Name: johnmandrus/package-detector

#Create an ubuntu image
FROM ubuntu
ENV DEBIAN_FRONTEND=noninteractive

#Update the base image
RUN apt-get update && apt-get -y update

#Install python and opencv
RUN apt-get install -y python3-pip python3-opencv curl mosquitto-clients

#Install packages
RUN pip install paho-mqtt
RUN pip3 install Cython
RUN pip3 install numpy

#Set the working directory
WORKDIR /app


#Copy and run package-detector.py + haar classifier
COPY package-detector.py package-detector.py
CMD ["python3", "package-detector.py"]