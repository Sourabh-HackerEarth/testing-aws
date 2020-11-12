# set base image (host OS)  #step - 1
FROM python:3.8

# set the working directory in the container #step - 2
WORKDIR /code

# copy the dependencies file to the working directory #step - 3
COPY requirements.txt .

# install dependencies
#step - 4
RUN pip install -r requirements.txt

# copy the content of the local src directory to the working directory
#step - 5
COPY src/ .

# command to run on container start
#step - 6
CMD [ "python", "./server.py" ]
