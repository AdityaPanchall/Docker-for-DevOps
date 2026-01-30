#Base image 
FROM python:3.12-slim 

#Creating Working Directory
WORKDIR /app

#Copying the source code to container 
COPY app.py ./app.py
COPY run.py ./run.py
COPY requirements.txt ./requirements.txt

#Install the system dependencies 
RUN pip install -r requirements.txt

#Expose Port 
EXPOSE 80

#Keep running the application
CMD ["python","run.py"]
