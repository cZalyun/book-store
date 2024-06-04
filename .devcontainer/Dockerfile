FROM mcr.microsoft.com/devcontainers/javascript-node:22-bookworm AS devcontainer

USER node
WORKDIR /workspace
RUN chown node:node /workspace

COPY --chown=node:node ./package*.json ./
RUN npm ci

COPY --chown=node:node ./ ./

CMD ["sleep", "infinity"]
