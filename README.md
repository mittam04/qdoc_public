# QDoc report generator

### Server requirements
1. Python >= 3.7
2. Git (Optional, if source code has already been downloaded)

## Installation (Optional steps)

> If you have the source and on your local machine and already configured a Python env you can skip this stage.

1. Clone the repo.
```sh
git clone git@github.com:mittam04/qdoc.git
```

2. Create a Python virtual env
```sh
python3 -m venv qdoc_py_env
```
3. Activate the env
```sh
source ./qdoc_py_env/bin/activate
```
4. Update or upgrade pip
```sh
pip install --upgrade pip
```
5. Install the dependencies for the project.
```sh
pip install -r requirements.txt
```


## How to run?

There are 2 input parameters required.

1. Directory name for the source files.
2. Directory name where the output should be.

```sh
python main.py source_dir_name output_dir_name contact_file_path
```

* `source_dir_name` is variable
* `output_dir_name` is variable
* `contact_file_path` is variable