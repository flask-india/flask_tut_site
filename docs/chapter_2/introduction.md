From a basic CRUD application you can laern a lot. Here **CRUD** means database operations **CR**eate, **U**pdate, **D**elete. As a developer its necessary to know these operations. We are using:

* **Flask-SQLAlchemy** for database operations
* **Flask-Migrate** for alembic `migrations`
* **Flask-WTF** for creating forms

Hopes readers will enjoy this chapter and learn a lot ahead database operations using this hands-on experiment. 

## Project Setup

Here we will create an Admin blueprint. We are not using any HTML templates for the explanation purpose. We will discuss about authentication, role-based login etc. in upcoming chapters.

```
flask_crud_app
├── app.py
└── flask_lib
    ├── admin
    │   ├── admin.py
    │   ├── admin_static
    │   │   └── style.css
    │   ├── admin_template
    │   │   ├── admin_base.html
    │   │   └── category_list.html
    │   ├── category.py
    │   ├── form
    │   │   └── category_form.py
    │   └── __init__.py
    └── __init__.py
```

## Installing Necessary Packages

As we mentioned earlier we need Flask-SQLAlchemy, Flask-Migrate and Flask-WTF

<div class="termy">
```console
$(venv) pip install Flask-SQLAlchemy Flask-Migrate Flask-WTF
---> 100%
```
</div>