# Use the latest Ubuntu image as the base image
FROM ubuntu:latest

# Update APT package list and upgrade packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix potential issue with EXTERNALLY-MANAGED
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory in the container
WORKDIR /app

# Copy the api.py file into the container
COPY api.py /app/api.py

# Command to run the Flask app
CMD ["python3", "api.py"]
