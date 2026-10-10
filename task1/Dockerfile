# Base image
FROM ubuntu:latest

# Update and upgrade installed packages
RUN apt-get update
RUN apt-get upgrade -y

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# Allow pip to install packages on externally managed environments
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask through pip3
RUN pip3 install flask

# Application directory
WORKDIR /app

# Copy the API source code
COPY ./api.py /app/api.py

# Start the Flask server
CMD ["python3", "/app/api.py"]
