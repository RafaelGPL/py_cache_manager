# Releasing

```
# Update version attribute in setup.py with <next version>
git tag <next version>
git push && git push --tags
rm -rf dist/*
python setup.py sdist bdist_wheel
twine upload dist/*
```
