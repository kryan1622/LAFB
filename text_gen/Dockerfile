FROM python
ARG FILE_VERSION=1
COPY . .
COPY text_gen${FILE_VERSION}.py app.py
RUN pip install flask
ENTRYPOINT ["python", "app.py"]
