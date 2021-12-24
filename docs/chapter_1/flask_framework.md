Flask is Python micro web framework. Flask is developed by **Armin Ronacher** on _April 1_, 2010. According to Ronacher, the idea was originally an April Fool's joke that was popular enough to make into a serious application. The name is a play on the earlier Bottle framework.

When Ronacher and Georg Brandl created a bulletin board system written in Python in 2004, the Pocoo projects Werkzeug and Jinja were developed.

In April 2016, the Pocoo team was disbanded and development of Flask and related libraries passed to the newly formed Pallets project.

### Flask Components

#### Werkzeug

Werkzeug (German for "tool") is a utility library for the Python programming language, in other words a toolkit for Web Server Gateway Interface (WSGI) applications, and is licensed under a BSD License. Werkzeug can realize software objects for request, response, and utility functions.

#### Jinja

Jinja, also by Ronacher, is a template engine for the Python programming language and is licensed under a BSD License. Similar to the Django web framework, it handles templates in a sandbox.

#### MarkupSafe

MarkupSafe is a string handling library for the Python programming language, licensed under a BSD license. The eponymous MarkupSafe type extends the Python string type and marks its contents as "safe"; combining MarkupSafe with regular strings automatically escapes the unmarked strings, while avoiding double escaping of already marked strings.

#### ItsDangerous

ItsDangerous is a safe data serialization library for the Python programming language, licensed under a BSD license. It is used to store the session of a Flask application in a cookie without allowing users to tamper with the session contents.

#### Click

Click is a beautiful, compasable command line interface (CLI) creation kit.

### Features

* Development server and debugger
* Integrated support for unit testing
* RESTful request dispatching
* Uses Jinja templating
* Support for secure cookies (client side sessions)
* 100% WSGI 1.0 compliant
* Unicode-based
* Extensive documentation
* Google App Engine compatibility
* Extensions available to enhance features desired