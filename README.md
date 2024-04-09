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
```