FROM python:3.11-buster

RUN pip install poetry==1.8.2

WORKDIR /home

COPY pyproject.toml poetry.lock ./
COPY app ./app
RUN touch README.md

RUN poetry install

ENTRYPOINT ["poetry", "run", "main"]