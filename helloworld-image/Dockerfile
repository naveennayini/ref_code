FROM ubuntu
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN pip install flask
COPY /home/ec2-user/ansible-test/helloworld-image/app.py /opt/app.py
ENTRYPOINT [ "FLASK_APP=/opt/app.py flask run --host=0.0.0.0" ]

