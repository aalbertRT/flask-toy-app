FROM python:3.7.3-stretch

# Set the working directory inside the container (create if not already existing)
WORKDIR /app

# Copy the content of the current folder 
ADD . /app

# Install app dependencies
RUN pip3 install -r requirements.txt
RUN pip3 install uwsgi

# Command to run the app
CMD ["uwsgi", "app.ini"]