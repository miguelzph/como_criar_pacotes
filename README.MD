# Criando pacotes em Python

## Como criar localmente?
```sh
pip install . # dentro da pasta package_file
```

<br><br>

## Como criar no Pypi test
```sh
python setup.py sdist # gera as pastas dist e distri_probability_tests.egg-info
pip install twine
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Instalando
```sh
pip install --index-url https://test.pypi.org/simple/ distri-probability-tests
```

<br><br>

## Como criar no Pypi
```sh
python setup.py sdist # gera as pastas dist e distri_probability_tests.egg-info
pip install twine
twine upload dist/*
```

### Instalando
```sh
pip install distri_probability_tests
```
