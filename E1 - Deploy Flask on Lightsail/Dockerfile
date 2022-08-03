# Set base image (host OS)
FROM python:3

# By default, listen on port 5000
EXPOSE 5000/tcp

# Set the working directory in the container
WORKDIR /app

# Install any dependencies
RUN pip install Flask

# Copy the content of the local src directory to the working directory
COPY app.py ./

# Specify the command to run on container start
CMD [ "python", "./app.py" ]
