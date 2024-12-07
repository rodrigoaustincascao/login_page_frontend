FROM node:20


RUN apt update && apt install -y less man-db sudo

RUN npm install @angular/cli -g


ARG USERNAME=node
RUN echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
    && chmod 0440 /etc/sudoers.d/$USERNAME


ENV DEVCONTAINER=true

EXPOSE 4200
