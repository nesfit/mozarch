FROM python:3.6

RUN apt update

RUN mkdir /Lemmiwinks

WORKDIR /Lemmiwinks
ADD ./lemmiwinks/ /Lemmiwinks
RUN python3 setup.py install && chmod +x ./pharty2/pharty2.py


RUN mkdir /MultiFIST
WORKDIR /MultiFIST

ADD ./multifist/ /MultiFIST
RUN mkdir media && pip install -r requirements.txt

