FROM mcr.microsoft.com/devcontainers/go:dev-1.24-bookworm

ENV GO111MODULE=on
ENV GOBIN=/usr/local/bin
ENV TERRAGRUNT_VERSION=v0.83.0
ENV DEVCONTAINER=true

USER root

RUN chown -R vscode:vscode /usr/local
RUN mkdir -p /workspace && chown -R vscode:vscode /workspace

# RUN echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://packages.cloud.google.com/apt cloud-sdk main" | tee -a /etc/apt/sources.list.d/google-cloud-sdk.list \
#   && curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | gpg --dearmor -o /usr/share/keyrings/cloud.google.gpg \
#   && apt-get update -y \
#   && apt-get install google-cloud-cli apt-utils -y

# RUN curl --proto '=https' --tlsv1.2 -fsSL https://get.opentofu.org/install-opentofu.sh -o install-opentofu.sh \
#   && chmod +x install-opentofu.sh \
#   && ./install-opentofu.sh --install-method deb \
#   && rm -f install-opentofu.sh

# RUN curl --proto '=https' --tlsv1.2 -fsSL https://github.com/gruntwork-io/terragrunt/releases/download/${TERRAGRUNT_VERSION}/terragrunt_linux_amd64 -o terragrunt \
#   && mv terragrunt /usr/local/bin/terragrunt \
#   && chmod +x /usr/local/bin/terragrunt

USER vscode