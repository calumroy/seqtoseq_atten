README.txt

# Docker container running tensorflow 2 GPU

# Notes ont his docker repo
To build make sure the current dir contains the Dockerfile and then use  

sudo docker build -t seqtoseq_atten:0.0.1 .

# To Run  
make sure nvidia-docker V2 is installed
This mounts the above directory

docker run --runtime=nvidia --rm -it -p 8888:8888 -p 4040:4040 --net=host -v $HOME/Documents/neural_nets/attention_seqtoseq_RNN/seqtoseq_atten:/home seqtoseq_atten:0.0.1 /bin/bash

#Run the notebook in the container
jupyter notebook --allow-root

