# Use Python 3.12 as the base image
FROM python:3.12-alpine

# Install git, openssl, and curl
RUN apk add --no-cache git openssl curl

# Define working directory
# WORKDIR /app

# Clone the Git repository
RUN git clone https://github.com/gallbotond/server-up.git

# Change directory to the cloned repository
WORKDIR /server-up

# Install dependencies
RUN pip install -r requirements.txt

# Get country and location information and store it in a file
# RUN curl -s https://ipinfo.io | grep -E '"country"|"region"' > location_info.txt

# # Expose port 5000
# EXPOSE 5000

# # Run the application
# CMD ["python", "./launch.py"]