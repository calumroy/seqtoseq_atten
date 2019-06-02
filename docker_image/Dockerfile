FROM tensorflow/tensorflow:latest-gpu-py3

# Make port 80 available to the world outside this container
EXPOSE 80

RUN pip install matplotlib
RUN pip install plotly
RUN pip install jupyter
RUN pip install sklearn

# Copy the above directory contents into the container at /home
#ADD . /home/seqtoseq_atten

# Set the working directory to /app
#WORKDIR /home/seqtoseq_atten

