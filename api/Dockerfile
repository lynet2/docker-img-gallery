FROM python:3.9

WORKDIR /app

EXPOSE 5050

# ./ = workdir
COPY Pipfile ./
COPY Pipfile.lock ./

RUN pip install pipenv
RUN pipenv lock  

COPY . ./

CMD ["python", "main.py"]