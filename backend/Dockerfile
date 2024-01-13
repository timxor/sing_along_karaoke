# Backend Dockerfile

# Use the official Python 3.12.1 image
FROM python:3.12.1

# Set the working directory in the container
WORKDIR /usr/src/backend

# Copy the dependencies file to the working directory
COPY requirements.txt .

# Install any dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the content of the local backend directory to the working directory
COPY . .

# Command to run the application
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]

