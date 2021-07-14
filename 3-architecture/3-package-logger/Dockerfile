#Image: johnmandrus/package-logger
FROM ubuntu:latest
# this is needed to make sure we can see the log output
ENV PYTHONUNBUFFERED=1
WORKDIR /app
RUN apt-get update && apt-get install -y python3 python3-pip
RUN pip3 install paho-mqtt
#RUN a command to intall the MQTT python client 
# Copy your package-logger.py file into the container
COPY package-logger.py package-logger.py
CMD ["python3", "package-logger.py"]