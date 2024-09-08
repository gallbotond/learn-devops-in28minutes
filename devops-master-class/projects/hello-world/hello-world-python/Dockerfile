# base image
FROM python:alpine3.10         

# define working directory    
WORKDIR /app                    

# install dependencies
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt

# expose port 5000
EXPOSE 5000                           

# copy all files from current directory to /app in container
COPY . /app          

# run the application
# CMD python ./launch.py
ENTRYPOINT ["python", "./launch.py"]

#COPY requirements.txt /app/requirements.txt
