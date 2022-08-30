FROM nvcr.io/nvidia/l4t-pytorch:r32.5.0-pth1.6-py3 


RUN apt-get update
RUN apt-get install -y git python3-pip libffi-dev cmake
RUN pip3 install packaging scikit-build
RUN pip3 install jupyter opencv-python
COPY entrypoint.sh /entrypoint.sh


ENTRYPOINT [ "/bin/bash", "/entrypoint.sh" ]
