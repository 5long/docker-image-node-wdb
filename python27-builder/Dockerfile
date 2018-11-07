FROM python:2.7-slim

RUN apt update && apt install -y --no-install-recommends curl build-essential
ENV CHANNEL=stable
RUN curl https://get.docker.com | bash
RUN rm -rf /var/lib/apt/lists/*
RUN curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py | python
RUN config.toml /root/.config/pypoetry/
