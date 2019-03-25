FROM pytorch/pytorch:1.0.1-cuda10.0-cudnn7-runtime

RUN pip install jupyter
RUN pip install 'ipykernel<5.0.0'

RUN adduser jovyan -q --disabled-password --gecos ""
RUN su jovyan
WORKDIR /homes/jovyan

EXPOSE 8888
USER 1000

CMD jupyter-notebook --ip=0.0.0.0
