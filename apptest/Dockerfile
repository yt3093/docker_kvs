From python:3.7.5-slim
RUN apt-get update && apt-get install -y iputils-ping net-tools
RUN pip install pytest==5.2.0 requests==2.22.0
WORKDIR /src
COPY ./src/test_app.py /src/test_app.py
ENV APP_HOST 127.0.0.1 
ENV APP_PORT 80
CMD ["tail", "-f", "/dev/null"]
