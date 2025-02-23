FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt /app/.
RUN pip install -r requirements.txt

EXPOSE 3141

CMD ["devpi-server", "--host", "0.0.0.0", "--port 3141"]
# devpi-server --init