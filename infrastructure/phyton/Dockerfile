FROM python:3.9

WORKDIR /backend

# 標準モジュールのインストール
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    build-essential \
    git \
    vim

# pip アップグレード
RUN pip install --upgrade pip

# Pythonライブラリのインストール
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt