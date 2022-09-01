# QDoc report generator


## Requirements
### Business
1. There should be a contact file by this name `contact.xlsx` at root project location.

2. Another folder with reports files should should in the root project location. 

### Server
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
python main.py source_dir_name output_dir_name
```

* `source_dir_name` is variable
* `output_dir_name` is variable


> Note: `contact.xlsx` must me in the root dir, not in the `source_dir_name`.