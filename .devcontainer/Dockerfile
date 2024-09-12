# Use an official Python runtime as a parent image
FROM python:3.11-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install make
RUN apt-get update && apt-get install -y make

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir poetry

# Make port 8501 available to the world outside this container
EXPOSE 8501

# Run make setup_admin_app when the container launches
CMD ["bash"]