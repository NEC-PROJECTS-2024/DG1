# Use an official Python runtime as a parent image
FROM python:3.10-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . .

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8000 to the outside world
EXPOSE 3000

# Run app.py when the container launches
ENTRYPOINT ["python3"]
CMD ["app.py", "runserver", "0.0.0.0:3000"]