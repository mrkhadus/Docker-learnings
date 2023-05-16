Step 1: Build image using command
    ~ docker build -t demo:first .
above command will create an image with the tag name = demo:first

Step 2: Create the container on top of the the image created above
cmd: docker run -p local-port:container-port imageName/imageId
image name= demo:first
    ~ docker run -p 3000:3000 --name demo-first-app demo:first
Done!

in browser url enter:
localhost:3000 
Why 3000? ==> We have opened the port 3000 while creating the
docker container and also the app listens to port 3000.