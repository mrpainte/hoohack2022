FROM localhost:32000/python3

RUN mkdir /app
WORKDIR /app
COPY ./requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY ./python/server.py server.py 

EXPOSE 8080

ENTRYPOINT ["python3", "server.py", "run", "--host=0.0.0.0"]
