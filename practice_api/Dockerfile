FROM python:3.8

# Define maintainer
MAINTAINER Eduardo Cervantes <ing.eduardocervantes@gmail.com>

# Environment variable for directory containing our app
ENV APP /app
ENV PYTHONUNBUFFERED 1

# Define working directory
RUN mkdir $APP

WORKDIR $APP

# Copy full rest repository
ADD . $APP

# Install missing dependencies
RUN pip install -r requirements.txt

# Expose default port
EXPOSE 8000
