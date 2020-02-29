FROM python:3.8

# Define maintainer
MAINTAINER Eduardo Cervantes <ing.eduardocervantes@gmail.com>

# Environment variable for directory containing our app
ENV PYTHONUNBUFFERED 1

# Define working directory
RUN mkdir /app

WORKDIR /app

COPY requirements.txt /app/

# Install missing dependencies
RUN pip install -r requirements.txt


# Copy full rest repository
COPY . /app/