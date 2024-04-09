# Create Pipenv environments


```console
mkdir resize_photos

cd resize_photos

pipenv --python 3

ipfile: /home/wayne/Pipfile
Using /usr/bin/python3 (3.10.12) to create virtualenv...
⠴ Creating virtual environment...created virtual environment CPython3.10.12.final.0-64 in 421ms
  creator CPython3Posix(dest=/home/wayne/.local/share/virtualenvs/wayne-ZnM5EoVx, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=/home/wayne/.local/share/virtualenv)
    added seed packages: pip==24.0, setuptools==69.1.1, wheel==0.43.0
  activators BashActivator,CShellActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator

✔ Successfully created virtual environment!
Virtualenv location: /home/wayne/.local/share/virtualenvs/wayne-ZnM5EoVx
```

## Activate pipenv shell
```console
pipenv shell
```

## Install bpython
```console
pipenv install bpython
```

## Manage Pipenv environments
```console
pipenv --rm

pipenv shell

pipenv install
Installing dependencies from Pipfile.lock

pipenv install requests
```

```console
pipenv check
Checking PEP 508 requirements...
Passed!
Checking Pipfile.lock packages for vulnerabilities...
+=============================================================================+

                               /$$$$$$            /$$
                              /$$__  $$          | $$
           /$$$$$$$  /$$$$$$ | $$  \__//$$$$$$  /$$$$$$   /$$   /$$
          /$$_____/ |____  $$| $$$$   /$$__  $$|_  $$_/  | $$  | $$
         |  $$$$$$   /$$$$$$$| $$_/  | $$$$$$$$  | $$    | $$  | $$
          \____  $$ /$$__  $$| $$    | $$_____/  | $$ /$$| $$  | $$
          /$$$$$$$/|  $$$$$$$| $$    |  $$$$$$$  |  $$$$/|  $$$$$$$
         |_______/  \_______/|__/     \_______/   \___/   \____  $$
                                                          /$$  | $$
                                                         |  $$$$$$/
  by pyup.io                                              \______/

+=============================================================================+

 REPORT 

  Safety v2.3.2 is scanning for Vulnerabilities...
  Scanning dependencies in your files:

  -> /tmp/resize_photos-OW5rojvV6xy7u3ni_requirements.txt

  Found and scanned 14 packages
  Timestamp 2024-04-09 14:52:07
  0 vulnerabilities found
  0 vulnerabilities ignored
+=============================================================================+

 No known security vulnerabilities found. 

+=============================================================================+
```

```console
pipenv graph
bpython==0.24
├── curtsies [required: >=0.4.0, installed: 0.4.2]
│   ├── blessed [required: >=1.5, installed: 1.20.0]
│   │   ├── six [required: >=1.9.0, installed: 1.16.0]
│   │   └── wcwidth [required: >=0.1.4, installed: 0.2.13]
│   └── cwcwidth [required: Any, installed: 0.1.9]
├── cwcwidth [required: Any, installed: 0.1.9]
├── greenlet [required: Any, installed: 3.0.3]
├── pygments [required: Any, installed: 2.17.2]
├── pyxdg [required: Any, installed: 0.28]
└── requests [required: Any, installed: 2.31.0]
    ├── certifi [required: >=2017.4.17, installed: 2024.2.2]
    ├── charset-normalizer [required: >=2,<4, installed: 3.3.2]
    ├── idna [required: >=2.5,<4, installed: 3.6]
    └── urllib3 [required: >=1.21.1,<3, installed: 2.2.1]
```

## Use Pipenv environments
```console
mkdir resize_photos_with_pipenv

cd resize_photos_with_pipenv/

cp ../resize_photos/requirements.txt

pipenv shell

pipenv run pip freeze
```