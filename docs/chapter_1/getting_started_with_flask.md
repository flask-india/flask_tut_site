Here we are introducing first flask application. Unlike django you can run flask application from a single file called `app.py`. You can give any name for this file. But flask internally recognizes `app.py` as a main flask application. so just go for that.

```py linenums="1" hl_lines="6-8"
from flask import Flask

app = Flask(__name__)


@app.route('/')
def index():
    return "Hello World"


if __name__ == '__main__':
    app.run()

```

The `app.py` is given above. In line number 1 we import Flask from flask package. In line number 3 we given `app = Flask(__name__)`. The `__name__` special python variable is given to Flask in order to get **import name**. This import name is essential because Flask finds out paths to `static` directory, `templetes` diretory and `blueprints` relative to this import name.

You can see highlighted function which is decorated with `app.route` method. The function decorated with `app.route` is called the **View function**. In the `app.route()` method we are defining url pattern for our `view`. Whatever the view function returns will become response of the route. Here view function returns a string which is `Hello World`. Hence `hello world` will be shown on browser.

## Run Flask Development Server

You can run flask development server using two methods.

### Method 1: Using Python Command

Navigate to your project directory using command prompt/ terminal. Activate virtual environment if you have virtual environnment. Then run flask application using following command:

For Windows:

<div class="termy">
```console
python app.py
```
</div>

For Linux:

<div class="termy">
```console
python3 app.py
```
</div>

### Using Flask Command Line Interface (CLI)

Flask comes with a nice command line interface using Pallet's Click Project. We can use command line interface in order to run our Flask Application.

* Setting Environment Variables

If you are not using name of the flask application as `app.py`, then Flask need to set atleast one environment variable. That environment variable `FLASK_APP`. If you are using name of application as `app.py` you can skip this step.

1\. Setting `FLASK_APP` environment variable

For Windows command prompt:
<div class="termy">
```console
set FLASK_APP=python_file_name_without_extension
```
</div>

???+ note
    For example, if our Flask application is saved in file `test.py`, then `python_file_name_without_extension` will becomes `test`.

For Windows Powershell:
<div class="termy">
```console
$env:FLASK_APP = "python_file_name_without_extension"
```
</div>

???+ warning
    Remember there is a double quoutes surrounding python_file_name_without_extension like `"python_file_name_without_extension"`.

For Linux:
<div class="termy">
```console
export FLASK_APP=python_file_name_without_extension
```
</div>

2\. Run Flask Application

You can run Flask application using following command.

<div class="termy">
```console
flask run
```
</div>

???+ success

    You can use any method for run Flask application. Since we didn't defined port the web server will run on default port (which is port 5000) of loop back address http://127.0.0.1:5000.

<figure markdown>
  ![output_1](/flask_tutorial/images/1.PNG){ width="300" }
  <figcaption>Example 1.1: Output</figcaption>
</fig>