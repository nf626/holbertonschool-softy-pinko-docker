# Is based on the latest ubuntu
FROM python:3.9-slim

WORKDIR /app
# Update APT using apt-get update
RUN apt-get update
# Upgrade currently installed software through APT using apt-get upgrade -y
RUN apt-get upgrade -y

# Install python3, python3-pip, and flask
# Note: Make sure to automatically install and skip user input with the -y flag for apt-get
# Note: flask must be installed with pip3, not through apt-get
RUN apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

RUN pip3 install flask flask-cors

COPY ./api.py /app/api.py

EXPOSE 5252

CMD [ "python3", "api.py" ]
