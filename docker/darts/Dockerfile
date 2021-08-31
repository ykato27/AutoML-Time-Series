FROM python:3.8.6-buster

WORKDIR /usr/src/app
ENV DEBIAN_FRONTEND noninteractive

# 必要なパッケージを記載
RUN apt-get update && apt-get install --no-install-recommends -y \
    curl && \
    apt-get clean

# 必要なPythonパッケージを記載
RUN python -m pip install --upgrade pip && pip install \ 
    numpy \
    scipy \
    matplotlib \
    ipython \
    scikit-learn \
    pandas \
    jupyterlab \
    ipywidgets

# Dartsのパッケージ
RUN pip install 'u8darts[all]'