# Use Python 3.6 or later as a base image
FROM python:3-alpine3.9
# Copy contents into image
# root/flaskApp
WORKDIR /flaskApp 
#Copies from dockerengine host cwd to container WORKDIR, which is set above
COPY . .
# Install pip dependencies from requirements
RUN pip install -r requirements.txt
RUN apk update
RUN apk add nginx 

#Don't need to restart service because container starts with all these changes, can be weird to visualise
# COPY nginx.conf /etc/nginx

# Set YOUR_NAME environment variable
ENV YOUR_NAME="Engineer"
# Expose the correct port
EXPOSE 5500/tcp
EXPOSE 80/tcp

# Create an entrypoint
ENTRYPOINT [ "python", "app.py" ]

#Run this with docker engine: docker build --tag 'tag-name' . (. represents cwd)