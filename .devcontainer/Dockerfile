FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y software-properties-common \ 
    && add-apt-repository ppa://waveform/ppa \ 
    && rm -rf /var/lib/apt/lists/* \
    && apt-get update \ 
    && apt-get install -y python-sense-emu python3-sense-emu sense-emu-tools

ARG USERNAME=codeany
RUN useradd -ms /bin/bash $USERNAME
USER $USERNAME

CMD ["tail", "-f", "/dev/null"]