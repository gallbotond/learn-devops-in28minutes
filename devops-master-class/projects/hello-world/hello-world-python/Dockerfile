 # base image
FROM python:alpine3.10         

# define working directory    
WORKDIR /app                            

# copy all files from current directory to /app in container
COPY . /app                             

# install dependencies
RUN pip install -r requirements.txt

# expose port 5000
EXPOSE 5000

# run the application
CMD python ./launch.py

#COPY requirements.txt /app/requirements.txt
#ENTRYPOINT ["python", "./launch.py"]
