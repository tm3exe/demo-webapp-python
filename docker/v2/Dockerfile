FROM python:3.6-slim
MAINTAINER tm3exe
RUN apt update && apt install -y git \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
RUN git clone https://github.com/tm3exe/demo-webapp-python.git
WORKDIR demo-webapp-python
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
EXPOSE 80
ENTRYPOINT python run.py
