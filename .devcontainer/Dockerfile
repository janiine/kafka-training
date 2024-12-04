FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update && apt-get install -y \
    python3 python3-pip wget curl docker.io \
    && apt-get clean

WORKDIR /workspace

# Download Kafka
RUN wget https://downloads.apache.org/kafka/3.5.0/kafka_2.13-3.5.0.tgz && \
    tar -xzf kafka_2.13-3.5.0.tgz && \
    mv kafka_2.13-3.5.0 kafka && \
    rm kafka_2.13-3.5.0.tgz
