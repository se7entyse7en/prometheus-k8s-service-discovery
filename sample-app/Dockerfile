FROM python:3.9

WORKDIR /app

RUN pip install poetry
COPY pyproject.toml .
RUN poetry config virtualenvs.create false && poetry install
COPY ./sample_app ./sample_app

CMD [ "python", "./sample_app/__init__.py" ]
