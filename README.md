# Tony's Example Package

[Tutorial Reference Link](https://packaging.python.org/en/latest/tutorials/packaging-projects/)

# Notes for self:
- git clone ... && cd ... && 
- pip install -e . or pip install -e ".[dev]"
- python -c "import my_package; print(my_package.__file__)"
- git commit -am "Prepare release v..."
- git tag -a v1.0.0 -m "Release v..."
- git push origin main --tags
- rm -rf dist
- pip install build twine 
- python -m build
- twine upload -r testpypi dist/*
- pip install dist/my_package-v0.0.0.whl
- python -c "import my_package; print(my_package.__file__)
- pip install -e .