# Use the official Python image as a base image
FROM python:3.10

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install dependencies
RUN pip install -r requirements.txt
# Expose the port number that the Flask app runs on
EXPOSE 5000

ENTRYPOINT ["python3"]
CMD ["app.py", "runserver", "0.0.0.0:5000"]