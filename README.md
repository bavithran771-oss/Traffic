# Traffic Level Predictor

A small Flask project that uses a decision tree to classify traffic as Low, Medium, or High from the hour and day. The CSV contains made-up practice examples.

## Run

```text
pip install -r requirements.txt
python app.py
```

Open the local address shown in the terminal.

## Run with Gunicorn

For a production-style server, install the dependencies and start the Flask app
with Gunicorn:

```text
pip install -r requirements.txt
gunicorn app:app
```

Gunicorn binds to `127.0.0.1:8000` by default. To make the app reachable from
other machines (for example, in a container), use:

```text
gunicorn --bind 0.0.0.0:8000 app:app
```
