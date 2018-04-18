![TND images](img/TND_coins.png)

# TND-Identifier - docker
Docker image that uses tensorflow to classify images of Tunisian currency


## Docker deployment
    $ docker build -t <your tag>/tnd-identifier .
    $ docker run it <yout tag>/tnd-identifier <image.xyz>


## Dependencies
    python3.x
    tensorflow
    opencv-python
    sklearn
    numpy