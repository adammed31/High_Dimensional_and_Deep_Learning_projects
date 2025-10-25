# Use an official Python runtime as the parent image
FROM pytorch/pytorch

# Set the working directory in the container to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY requirements.txt /app

# Install git
RUN apt-get update && apt-get install -y git

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make this port available for notebook
EXPOSE 8888