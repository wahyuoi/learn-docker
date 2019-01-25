# base image
FROM python:2.7-slim

# working directory
WORKDIR /app

# copy current directory contents into container at /app
COPY . /app

# install python packages
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# expose port 80 to outside this container
EXPOSE 80

# define env variable
ENV NAME World

# run app.py 
CMD ["python", "app.py"]

