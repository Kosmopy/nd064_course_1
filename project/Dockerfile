FROM python:3.8
LABEL maintainer="Kosmopy"

COPY ./techtrends/requirements.txt ./

RUN pip install -r requirements.txt

COPY ./techtrends ./

RUN python init_db.py

EXPOSE 3111

# command to run on container start
CMD [ "python", "init_db.py" ]
