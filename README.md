# django-create-react-app


## Create an app


## 1. Call create-react-app command

```
./manage.py startreactapp polls
```

That’ll create a directory polls, which is laid out like this:

```
polls/
    __init__.py
    package.json
    src/
        App.js
        App.test.js
        index.css
        logo.svg
        index.js
        App.css
```

## 2. Add polls to your project

```python
INSTALLED_APPS = [
    'polls',
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
]
```

## 3. Load polls

```htmldjango
{% load polls %}

<head>
  <link rel="stylesheet" href="{% polls.style %}">
</head>
<body>
  <script src="{% polls.script %}"></script>
</body>
```


