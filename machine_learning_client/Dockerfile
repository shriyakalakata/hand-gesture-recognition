# docs: https://hub.docker.com/_/python
FROM python:3.10

WORKDIR /machine_learning_client

RUN apt-get update && apt-get install ffmpeg libsm6 libxext6  -y

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "app.py" ]