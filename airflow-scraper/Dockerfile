# Use the official Airflow image as the base
FROM apache/airflow:2.7.0-python3.10
USER airflow
# Copy the requirements.txt file into the container
COPY requirements.txt /requirements.txt

# Install additional Python dependencies
RUN pip install --no-cache-dir -r /requirements.txt

ENV PYTHONPATH=/home/airflow/.local/lib/python3.10/site-packages
