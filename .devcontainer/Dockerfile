FROM python:3.10
USER root
WORKDIR /workspace

RUN apt-get update && \
    apt-get -y install --reinstall ca-certificates && \
    apt-get -y install software-properties-common \
    chromium \
    chromium-driver \
    xclip && \
    pip install --upgrade pip

# Install Basic Packages
RUN pip install ipykernel jupyter

COPY ../requirements.txt /workspace/
Run pip install -r requirements.txt