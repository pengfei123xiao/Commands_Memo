## Install dependencies
1. git clone the repo: **git clone xxxxxxx**
2. install 'virtualenv' package. **sudo pip install virtualenv**
3. create a virtual environment: **virtualenv venv_<name>**
4. go into the virtual environment: for windows user: **venv\Scripts\activate**; for Mac/Linux user: **source venv_<name>/bin/activate**
5. run **(sudo) pip install -r requirements.txt** (to install all dependencies)
- (when meet mysql_config error, try: `sudo apt install libmysqlclient-dev`)
6. leave venv via: **deactivate**
