FROM mcr.microsoft.com/vscode/devcontainers/base:debian-11

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
&& apt-get -y install --no-install-recommends vim

COPY .bashrc /home/vscode/.bashrc

USER vscode
RUN curl -fsSL https://deno.land/x/install/install.sh | sh
RUN sudo ln -s /home/vscode/.deno/bin/deno /usr/local/bin/deno