# Use Python 3.10 as the base image
FROM python:3.10-slim

# Set the working directory
WORKDIR /app

# Install required Python package
RUN pip install --no-cache-dir prometheus-client

# Copy the Python application
COPY delivery_metrics.py .

# Expose the Prometheus metrics port
EXPOSE 8000

# Start the application
CMD ["python", "delivery_metrics.py"]