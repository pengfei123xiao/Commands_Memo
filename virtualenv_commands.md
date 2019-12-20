## Analytics Repo dependencies
1. git clone the repo: `git clone xxxxxxx`
2. install 'virtualenv' package. `sudo pip install virtualenv`
3. create a virtual environment in `dashboard/python` directory (need to match `.gitignore`): `virtualenv env -p python2.7`
4. go into the virtual environment: for windows user: `env\Scripts\activate`; for Mac/Linux user: `source env/bin/activate`
5. run `pip install -U pip wheel; pip install -r requirements.txt` (to install all dependencies)
- (when meet mysql_config error, try: `sudo apt install libmysqlclient-dev`)
6. leave venv via: **deactivate**


## Dissect Repo dependencies
1. git clone the repo: `git clone xxxxxxx`
2. install 'virtualenv' package. `sudo pip install virtualenv`
3. create a virtual environment in root directory: `virtualenv venv -p python3`
4. go into the virtual environment: for windows user: `venv\Scripts\activate`; for Mac/Linux user: `source venv/bin/activate`
5. run `pip install fl_dbconnect --extra-index-url https://nexus.tools.flnltd.com/repository/pypi/simple; python setup.py develop` (to install all dependencies)
- (when meet postgresql-server-dev-X.Y error, try: 
```
sudo apt-get install postgresql
sudo apt-get install python-psycopg2
sudo apt-get install libpq-dev
```)

6. leave venv via: **deactivate**
