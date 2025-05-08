# Tony's Example Package

[Tutorial Reference Link](https://packaging.python.org/en/latest/tutorials/packaging-projects/)

# Notes for self:
- git clone 
- or pip install -e git+https://github.com/numpy/numpy.git@v1.25.0#egg=numpy
- or pip install -e git+https://github.com/owner/repo.git@branch#egg=package
- or pip install -e git+https://@github.com/owner/repo.git@branch#egg=package_name
- or pip install -e git+ssh://git@github.com/owner/repo.git@main#egg=private_pkg
- add venv 
- pip install -e .
- or pip install -e ".[dev]"
- python -c "import my_package; print(my_package.__file__)"
- git commit -am "Prepare release v..."
- git tag -a v1.0.0 -m "Release v..."
- or git push origin main --tags
- or git push origin v...
- git push origin main --tags
- rm -rf dist
- [if not in backend build] pip install build twine 
- [if not in backend build] python -m build
- twine upload -r testpypi dist/*
- pip install dist/my_package-v0.0.0.whl
- python -c "import my_package; print(my_package.__file__)
- pip install -e .
