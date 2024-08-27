# Use the latest version of Ubuntu as the base image
FROM ubuntu:latest

# Update and upgrade the APT package manager
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix for externally managed Python environments in some base images
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory for the container
WORKDIR /app

# Copy the Flask app file into the container
COPY api.py /app/

# Set environment variable for the Flask application
ENV FLASK_APP=api.py

# Command to run the Flask app
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=5252"]