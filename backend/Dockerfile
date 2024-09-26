# Dockerfile for Flask
# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the requirements.txt file and install dependencies
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# Copy the rest of the application code
COPY . .

# Define environment variable for Flask
ENV FLASK_APP=flaskr/app.py

# Expose the port that Flask will run on
EXPOSE 5000

# Set the command to run the Flask application
CMD ["python", "app.py"]