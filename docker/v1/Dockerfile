FROM python:3.6
MAINTAINER tm3exe
RUN apt update
RUN apt install -y git
RUN git clone https://github.com/tm3exe/demo-webapp-python.git
WORKDIR demo-webapp-python
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
EXPOSE 80
ENTRYPOINT python run.py
