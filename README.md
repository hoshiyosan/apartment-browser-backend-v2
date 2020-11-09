
## Development

### Requirements

- docker
- docker-compose
- pipenv

### Install dev. dependencies

It is recommended that you add this to your bashrc or in your current 
terminal to create virtualenv in your project.
Otherwise your IDE won't be able to lint correctly.
```
export PIPENV_VENV_IN_PROJECT=1
```

Then install dependencies in a virtualenv using
```
pipenv install
```

### Setup additional services

To quickly run services required by backend on your local machine, run
```
docker-compose up
```

It will bring up :
- a mongo database on http://localhost:27017
- a mongo web ui on http://localhost:1234

These values are the default ones in `settings.py` when not overriden by environment variables.

### Run backend



```
pipenv run serve
```
