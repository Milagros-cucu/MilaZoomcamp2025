
FROM python:3.12

RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2 pyarrow

WORKDIR /app
COPY data_ingest.py data_ingest.py

ENTRYPOINT [ "python", "data_ingest.py" ]

# $ docker run -it python:3.12.8 bash
# $ pip --version
# -> pip 24.3.1 from /usr/local/lib/python3.12/site-packages/pip (python 3.12)

