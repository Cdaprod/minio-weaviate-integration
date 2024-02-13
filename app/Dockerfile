FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt /app/
RUN pip install weaviate-client
COPY python_initializer.py entrypoint.sh /app/
RUN chmod +x /app/entrypoint.sh
ENTRYPOINT ["/app/entrypoint.sh"]
