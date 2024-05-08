#Tells Docker to use this Node version
FROM node:22.1.0

#Tells Docker to create folder called code inside Docker image
WORKDIR /code

#Environemnt variables can be accessed inside image
ENV  PORT 80

#Copies the package.json file into code folder
COPY package.json /code/package.json

#Runs node package manager and install dependencies
RUN npm install

#Copies all code from current working directory into code directory in image
COPY . /code




# First step
# npm init -y

# Incase Json file is not generating after npm init -y
# Set-ExecutionPolicy RemoteSigned  (in Powershell (Admin))

# To build the docker file
# docker build -t my-node-app .

# To build the docker file
# docker run -p 8000:80 my-node-app