# docker_web_app

## Step 1 : Clone the repository.
           $git clone https://github.com/nouman-atac/docker_web_app.git

## Step 2: cd into the directory
           $cd docker_web_app

## Step 3: Edit file so the output looks different.
           Edit the file app.js  --> change "Hello World to something else"
           
## Step 4: Build docker image
           $ docker build . -t <yourname>/web-app:latest

## Step 5: Run docker container from image
          Use any one:
          
          a)Works for both windows and linux
           $ docker run -it -p 3000:3000 <yourname>/web-app:latest
           
          b)Works for linux only
           $ docker run -it -p 3000:3000 -v "$(pwd)":/app <yourname>/web-app:latest
## Step 6: Open http://localhost:3000/ in browser.
