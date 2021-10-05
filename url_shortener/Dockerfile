From python:latest

WORKDIR /code

COPY requirements.txt /code/

RUN pip install -U pip 
RUN pip install -r requirements.txt

COPY . /code/

CMD ["gunicorn", "url_shortener.wsgi", ":8000"]