FROM python:3.9

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip -y
RUN pip install jupyter

WORKDIR /workspace/jupyter

CMD ["jupyter", "notebook", "--ip", "0.0.0.0", "--port", "8888", "--allow-root", "--NotebookApp.token='12345'"]
