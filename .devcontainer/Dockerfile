# Gunakan base image Python resmi
FROM python:3.11-slim

# Set working directory di dalam container
WORKDIR /app

# Copy file requirements dan install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy sisa source code ke dalam container
COPY . .

# Perintah default (opsional)
CMD ["python", "src/agent-IoX/agent.py"]