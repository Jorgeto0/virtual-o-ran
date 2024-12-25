# Use Python base image
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy application files
COPY app.py .

# Install Flask
RUN pip install flask

# Expose the container port
EXPOSE 8080

# Run the app
CMD ["python", "app.py"]
