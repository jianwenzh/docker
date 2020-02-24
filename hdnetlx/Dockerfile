FROM nvidia/cuda:10.0-cudnn7-devel-ubuntu18.04
RUN apt-get update && apt-get install -y apt-utils python3.7 python3-pip 
Add ./requirements.txt .
RUN ln -s /usr/bin/python3 /usr/bin/python & \
    ln -s /usr/bin/pip3 /usr/bin/pip
RUN pip install -r requirements.txt
RUN python -m spacy download en_core_web_lg
