We can install Flask using any package manager like pip, pipenv, virtualenv etc. But here we are demonstrating installation with python pip package manager.

## Installation on Windows

1\. Navigate to project folder using `cd` command.

<div class="termy">
```console
cd path\to\project_dir\
```
</div>

2\. Create virtual environment

<div class="termy">
```console
python -m venv venv
```
</div>

here last `venv` is the name of virtual environment. You can change the name of virtual environment if you wish. However it will create a `venv` folder inside your project folder.

???+ warning

    If you running your project on Windows or Linux, ensure the virtual environment is enabled. Unless you will end up with `ImportError` no module named Flask. 

3\. Activate virtual environment

<div class="termy">
```console
.\venv\Scripts\activate
```
</div>

4\. Install Flask

<div class="termy">
```console
(venv)path\to\project_dir> pip install flask
---> 100%
```
</div>

## Installation on Linux

1\. Navigate to project folder using `cd` command.

<div class="termy">
```console
$ cd path/to/project_dir
```
</div>

2\. Create virtual environment

<div class="termy">
```console
$ python3 -m venv venv
```
</div>

here last `venv` is the name of virtual environment as mentioned earler.

3\. Activate virtual environment

<div class="termy">
```console
source venv/bin/activate
```
</div>

4\. Install Flask

<div class="termy">
```console
(venv)path/to/project_dir> pip3 install flask
---> 100%
```
</div>