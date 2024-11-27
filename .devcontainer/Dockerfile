FROM python:3.10.10
WORKDIR /work
COPY requirements.txt .
RUN apt-get update && apt-get install -y \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
RUN pip install --no-cache-dir -r requirements.txt