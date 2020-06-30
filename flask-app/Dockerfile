#Use Python Image
FROM python:3.8
RUN apt update
RUN apt install python3-pip -y
 
# Copy contents into image

COPY . . 
# run pip dependencies
RUN pip3 install PyMySQL==0.9.3 Flask-SQLAlchemy==2.4.3 SQLAlchemy==1.3.17 Jinja2==2.11.2 Flask==1.1.2
RUN pip3 install cryptography 
 

# Expose correct port

EXPOSE 5000

# Create an entrypoint


ENTRYPOINT ["/usr/local/bin/python3", "app.py"]
