FROM python:3.7-slim

# Copy local code to the container image.
ENV /app
COPY . .

# Install production dependencies.
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

EXPOSE 8080

ENTRYPOINT ["python", "app.py"]
