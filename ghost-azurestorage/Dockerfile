FROM bitnami/ghost:latest

USER root

RUN npm install ghost-azure-storage --unsafe-perm \
    && cp -vR node_modules/ghost-azure-storage ./current/core/server/adapters/storage

