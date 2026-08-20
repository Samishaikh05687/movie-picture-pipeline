FROM python:3.10-slim

ENV FLASK_RUN_HOST=0.0.0.0
ENV PIP_NO_CACHE_DIR=1
ENV PIPENV_NOSPIN=1

WORKDIR /app

RUN useradd -u 1000 -m app

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    build-essential \
    gcc \
    python3-dev \
    libpcre3 \
    libpcre3-dev \
    && rm -rf /var/lib/apt/lists/*

RUN pip install --upgrade pip && \
    pip install pipenv

COPY Pipfile Pipfile.lock ./

RUN pipenv sync --system

COPY . .

RUN chown -R app:app /app

USER app

CMD ["uwsgi", "--http", ":5000", "--master", "--enable-threads", "--manage-script-name", "--mount", "/=app:app"]