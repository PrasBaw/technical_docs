- pip show packagename  # To get package version -------
- pip install -e . --force-reinstall

- pip install coverage
coverage run -m pytest
coverage report --fail-under=60

Modules and Pacakges:
	Modules are .py files.
		if __name__== '__main__'
	Packages are folder containing an 
		__init__.py
		This should always be empyty
	Directory structure should be API
