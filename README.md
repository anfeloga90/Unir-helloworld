# Repo para EU - DevOps&Cloud - UNIR

Este repositorio incluye un proyecto sencillo para demostrar los conceptos de pruebas unitarias, pruebas de servicio, uso de Wiremock y pruebas de rendimiento
El objetivo es que el alumno entienda estos conceptos, por lo que el código y la estructura del proyecto son especialmente sencillos.
Este proyecto sirve también como fuente de código para el pipeline de Jenkins.

## Comandos ejecutados.

Instalar dependencias

***`apt install python3-flask`***

**`apt install openjdk-11-jre-headless`**

**`apt install python3-pip`**

**`pip install pytest`**

***`pip install flask`***

***`export FLASK_APP=app/api.py`***

**`export PYTHONPATH=$(pwd)`**

***flask run***

* Serving Flask app 'app/api.py' (lazy loading)
* Environment: production
  WARNING: This is a development server. Do not use it in a production deployment.
  Use a production WSGI server instead.
* Debug mode: off
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)

***java -jar wiremock-jre8-standalone-2.33.1.jar --port 9090 --root-dir test/wiremock/ --verbose***

## Ejecutar pruebas

pytest test/rest

========================== test session starts ===========================
platform darwin -- Python 3.9.12, pytest-7.1.2, pluggy-1.0.0
rootdir: /Users/andresfelipelopezgallego/Documents/Documentos - MacBook Pro/Git/python/UNIR/JENKIS/Unir-helloworld, configfile: pytest.ini
plugins: anyio-3.4.0
collected 2 items

test/rest/api_test.py ..                                                                                                                  [100%]

=========================== 2 passed in 0.06s ===============================

pytest test/unit
