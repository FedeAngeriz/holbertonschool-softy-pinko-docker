FROM ubuntu:latest

RUN apt-get update && apt-get update -y

RUN apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

RUN pip3 install flask-cors

COPY api.py /app/api.py

WORKDIR /app

EXPOSE 5252

CMD ["python3", "api.py"]
