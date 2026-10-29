FROM python:3.12-bookworm

WORKDIR /tasks-api

COPY requirements.txt .

RUN ["pip", "install", "-r", "requirements.txt"]

COPY . .

EXPOSE 5000

CMD ["flask", "--app", "app:create_app", "run", "--host", "0.0.0.0", "--port", "5000"]

