FROM mcr.microsoft.com/devcontainers/go:dev-1.25-bookworm

ENV GO111MODULE=on
ENV GOBIN=/usr/local/bin
ENV DEVCONTAINER=true

USER root

RUN chown -R vscode:vscode /usr/local
RUN mkdir -p /workspace && chown -R vscode:vscode /workspace

USER vscode