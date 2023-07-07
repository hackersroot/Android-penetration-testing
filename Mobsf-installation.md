# In Pc
$ git clone https://github.com/MobSF/Mobile-Security-Framework-MobSF.git
$ sudo apt-get install git-all
$ cd Mobile-Security-Framework-MobSF
$ pip install -r requirements.txt
$ ./setup.sh
##--Got Error--##
[ERROR] MobSF dependencies require Python 3.8/3.9.
Try
$ sudo apt-get update
$ mkdir ~/tmp
$ cd ~/tmp
$ wget https://www.python.org/ftp/python/3.9.0/Python-3.9.0.tgz
$ tar -xvzf Python-3.9.0.tgz
$ cd Python-3.9.0
$ ./configure
$ sudo make install
Again
$ ./setup.sh
$ ./run.sh 127.0.0.1:8000
