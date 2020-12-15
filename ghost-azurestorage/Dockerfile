FROM bitnami/ghost:latest

USER root
RUN npm install ghost-azure-storage --unsafe-perm
RUN useradd ghost
RUN echo "ghost ALL=(ALL:ALL) NOPASSWD: ALL" | tee /etc/sudoers.d/ghost
RUN cp -vR node_modules/ghost-azure-storage ./current/core/server/adapters/storage
