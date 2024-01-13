# Frontend Dockerfile

# Use the official Node.js 21.4.0 image
FROM node:21.4.0 AS build

# Set the working directory in the container
WORKDIR /usr/src/frontend

# Install Yarn only if it's not already installed
RUN if ! [ -x "$(command -v yarn)" ]; then \
        npm install --global yarn; \
    fi

# TODO
# Copy package.json and yarn.lock
# COPY package.json yarn.lock ./

# TODO
# Install dependencies
# RUN yarn install

# TODO
# Copy the content of the local frontend directory to the working directory
# COPY . .

# TODO
# Build the app (if necessary)
# RUN yarn build

# Stage 2: Run stage
FROM node:21.4.0

WORKDIR /usr/src/frontend

COPY --from=build /usr/src/frontend .

# Create a user and switch to it
RUN useradd -m myuser
USER myuser

# Expose the port the app runs on
EXPOSE 3000

# Command to run the app
CMD ["yarn", "start"]
