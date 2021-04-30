#FROM ubuntu:18.04
FROM python:3.9

ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=America/New_York

EXPOSE 8501

ADD requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

WORKDIR /app
COPY . .

CMD ["streamlit", "run", "streamlit_app.py"]