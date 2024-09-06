### Create a Project

```bash
jango-admin startproject myproject
```

This will create a "myproject" folder with the following structure −

```tree
root
├── myproject
│ ├── myproject
│ │ ├── **init**.py
│ │ ├── asgi.py
│ │ ├── settings.py
│ │ ├── urls.py
│ │ └── wsgi.py
│ ├── db.sqlit3
│ └── manage.py
├── .gitignore
└── README.md
```

### The Project Structure

The `myproject` folder is just your project container, it actually contains two elements −

- **`manage.py`** − This file is kind of your project local django-admin for interacting with your project via command line (start the development server, sync db...). To get a full list of command accessible via manage.py you can use the code −

```bash
python manage.py help
```

- **The `myproject` subfolder** − This folder is the actual python package of your project. It contains four files −
  - **init.py** − Just for python, treat this folder as package.
  - **settings.py** − As the name indicates, your project settings.
  - **urls.py** − All links of your project and the function to call. A kind of ToC of your project.
  - **wsgi.py** − If you need to deploy your project over WSGI. As like the same **`ASGI`**.
  - **WSGI** stand for
    - W = Web
    - S = Server
    - G = Gateway
    - I = Interface
