FROM cypress/base

# Set the current working directory inside the image
WORKDIR /app

COPY ./cypress ./cypress
COPY ./cypress.json ./cypress.json

RUN export DOCKER_BUILDKIT=0
RUN export COMPOSE_DOCKER_CLI_BUILD=0

RUN npx cypress run

