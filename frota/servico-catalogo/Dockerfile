FROM python:3.12.3-slim

WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

RUN useradd --uid 1000 --create-home app
USER app

EXPOSE 8080
CMD ["python", "app.py"]
