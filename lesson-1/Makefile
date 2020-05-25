setup:
	python3 -m venv microservices

install:
	pip install -r requirements.txt

test:
	python -m pytest -vv --cov=microserviceslib tests/*.py
	python -m pytest --nbval notebook.ipynb


lint:
	pylint --disable=R,C microserviceslib cli web

all: install lint test