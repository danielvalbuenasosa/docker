#Use python
FROM python:2.7-slim

#Working dir to app
WORKDIR /app

# Copy current diractory contents to app
ADD . /app

#Install any needed packages specified
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make port 80 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

#RUN app.py when the container launches
CMD ["python", "app.py"]
