# docker_web_app


## Step 1: Edit File so that the output looks different

## Step 2: Build docker image
           $ docker build . -t <yourname>/web-app:latest

## Step 3: Run docker container from image
          Use any one:
          
          a)Works for both windows and linux
           $ docker run -it -p 3000:3000 <yourname>/web-app:latest
           
          b)Works linux only
           $ docker run -it -p 3000:3000 -v "$(pwd)":/app <yourname>/web-app:latest
