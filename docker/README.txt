- To start:

docker build -t gui-container .

- To run app:

docker run -it --rm --name gui-app \
    --net=host \
    -e DISPLAY=$DISPLAY \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    gui-container

xcalc

- To exit:

exit