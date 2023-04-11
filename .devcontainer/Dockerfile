FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

RUN sudo add-apt-repository ppa://waveform/ppa && sudo apt-get update && sudo apt-get install -y python-sense-emu python3-sense-emu sense-emu-tools

ARG USERNAME=codeany
RUN useradd -ms /bin/bash $USERNAME
USER $USERNAME

CMD ["tail", "-f", "/dev/null"]