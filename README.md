# QDoc report generator

## Description

This script downloads monthly reports from [Literature PPI reports 2022](https://pfizer.sharepoint.com/sites/SER-VM-Partners/Parexel/Forms/AllItems.aspx?RootFolder=%2Fsites%2FSER%2DVM%2DPartners%2FParexel%2FOthers%2FLiterature%2FLiterature%20PPI%20reports%202022&View=%7BAE064FBB%2DB26D%2D4DE5%2D96D0%2D2F58D29D3AA8%7D) and generates a customized consolidated report.


## Overview of script execution
The script will always check for reports for **current month**. And if the folder for current month is not present, then it will look for the previous month.

If the previous month folder is found then, it will start working on that folder. Else the **script will quit**.

## Requirements
### Business
1. There should be `only 1` contact file with `.xlsx` extension in [this](https://pfizer.sharepoint.com/sites/SER-VM-Partners/Parexel/Forms/AllItems.aspx?RootFolder=%2Fsites%2FSER%2DVM%2DPartners%2FParexel%2FOthers%2FLiterature%2FQDOC%5FSSLR%5FImport%5F2022%2FContactlist&FolderCTID=0x012000DB328F25E534724A8672B53AEB39AE5B&View=%7BAE064FBB%2DB26D%2D4DE5%2D96D0%2D2F58D29D3AA8%7D) location. (Script will not parse any other extension)

2. Raw reports files should be in [this](https://pfizer.sharepoint.com/sites/SER-VM-Partners/Parexel/Forms/AllItems.aspx?RootFolder=%2Fsites%2FSER%2DVM%2DPartners%2FParexel%2FOthers%2FLiterature%2FLiterature%20PPI%20reports%202022&FolderCTID=0x012000DB328F25E534724A8672B53AEB39AE5B&View=%7BAE064FBB%2DB26D%2D4DE5%2D96D0%2D2F58D29D3AA8%7D) location. The format should be same as it is now.

### Server
1. Sharepoint credentials
    - Email
    - Password
2. Linux server
3. Python >= 3.7
4. Git

## Installation
1. Clone the repo from [here](git@github.com:mittam04/qdoc.git). (This is a temporary location).
```sh
$ git clone git@github.com:mittam04/qdoc.git
```
2. Go to the repo
```sh
$ cd qdoc
```
3. Create a Python virtual env
```sh
$ python3 -m venv qdoc
```
4. Activate the env
```sh
$ source ./qdoc/bin/activate
```
5. Update or upgrade pip
```sh
$ pip install --upgrade pip
```
6. Install the dependencies for the project.
```sh
$ pip install -r requirements.txt
```
7. Copy the `config.py.template` to `config.py`
```sh
$ cp config.py.template config.py
```
8. Replace the credentials
9. Run the script
```sh
$ python main.py
```

## Results
After execution generated reports will be in [this](https://pfizer.sharepoint.com/sites/SER-VM-Partners/Parexel/Forms/AllItems.aspx?RootFolder=%2Fsites%2FSER%2DVM%2DPartners%2FParexel%2FOthers%2FLiterature%2FQDOC%5FSSLR%5FImport%5F2022&FolderCTID=0x012000DB328F25E534724A8672B53AEB39AE5B&View=%7BAE064FBB%2DB26D%2D4DE5%2D96D0%2D2F58D29D3AA8%7D) location.
