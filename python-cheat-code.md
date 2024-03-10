- pip show packagename  # To get package version -------
- pip install -e . --force-reinstall

- pip install coverage
coverage run -m pytest
coverage report --fail-under=60
