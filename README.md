# Albumy

*Capture and share every wonderful moment.*

> Example application for *[Python Web Development with Flask](https://helloflask.com/en/book/1)* (《[Flask Web 开发实战](https://helloflask.com/book/1)》).

Demo: http://albumy.helloflask.com

![Screenshot](https://helloflask.com/screenshots/albumy.png)

## Installation

clone:
```
$ git clone https://github.com/greyli/albumy.git
$ cd albumy
```
create & activate virtual env then install dependency:

with venv/virtualenv + pip:
```
$ python -m venv env  # use `virtualenv env` for Python2, use `python3 ...` for Python3 on Linux & macOS
$ source env/bin/activate  # use `env\Scripts\activate` on Windows
$ pip install -r requirements.txt
```
or with Pipenv:
```
$ pipenv install --dev
$ pipenv shell
```
generate fake data then run:
```
$ flask forge
$ flask run
* Running on http://127.0.0.1:5000/
```
Test account:
* email: `admin@helloflask.com`
* password: `helloflask`

## Auto Captioning and Auto Tagging Feature
Albumy now supports automatic captioning and tagging of uploaded images using the Azure Computer Vision API.

### Connecting to the Azure Vision API

1. Sign up for a student account for Microsoft Azure: https://azure.microsoft.com/en-us/free/students/ – no credit card required.
2. Create an instance of the Computer Vision service and obtain the API endpoint for your service instance.
3. Get a subscription key to authorize your script to call the Computer Vision API.
4. Update your application code with the obtained endpoint and key.
5. Ensure you have installed all necessary dependencies from `requirements.txt` using:
   ```
   $ pip install -r requirements.txt
   ```
6. Run the application and test the automatic captioning and tagging feature.

## License

This project is licensed under the MIT License (see the [LICENSE](LICENSE) file for details).

