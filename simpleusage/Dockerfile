# Use an official Python runtime as a parent image
FROM python:2.7-slim

# Set the working directory to /mydatetime
WORKDIR /mydatetime

# Copy the current directory contents into the container at /app
ADD . /mydatetime

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

# Run mydatetime.py when the container launches
CMD ["python", "mydatetime.py"]

