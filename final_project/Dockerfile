FROM python:3.8-slim-buster

WORKDIR /app

COPY requirements.txt requirements.txt

RUN python3 -m pip install --upgrade pip
RUN python3 -m pip install -r /app/requirements.txt

COPY . .

CMD ["python3", "-m", "flask", "run", "--host:0.0.0.0"]