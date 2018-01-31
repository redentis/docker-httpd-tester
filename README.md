# Apache 2 Testing 
## Background

## Getting Started

1. Modify the Apache config file (httpd.conf) if necessary
1. Create or replace the content for testing in the `www` folder    
1. Build a docker image 

       $ docker build -t {image-name} .
1. Start the new image
       
       $ docker run -dit --name {container-name} {image-name} .

If you need to connect to the running container to check logs etc.

       $ docker exec -i -t {container-name} /bin/bash