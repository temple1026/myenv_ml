FROM tensorflow/tensorflow:2.3.0-gpu

RUN apt-get update && apt-get install -y git

RUN pip3 install scikit_learn scipy

RUN apt-get clean && apt-get autoremove