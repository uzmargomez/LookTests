#FROM ubuntu:18.04
FROM ubuntu:20.04

EXPOSE 8501

RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y cmake python3-pip 
RUN pip3 install --upgrade pip
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt

WORKDIR /app
COPY . .

CMD ["streamlit", "run", "streamlit_app.py"]