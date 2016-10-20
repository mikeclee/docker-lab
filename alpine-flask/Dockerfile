FROM alpine:latest

RUN apk add --update py-pip

COPY requirements.txt /usr/src/app/
COPY app.py /usr/src/app/
COPY templates/ /usr/src/app/templates

RUN pip install --no-cache-dir -r /usr/src/app/requirements.txt

EXPOSE 5000

CMD [ "python", "/usr/src/app/app.py" ]
