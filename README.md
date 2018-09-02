# gen_logs

This is to simulate web application writing traffic details to log file.

* It has shell scripts which invoke python program
* It is compatible with Python 3

Here is the setup process on linux or mac or on cygwin.

* Identify directory /opt/
* Copy gen_logs directory to /opt
* Run sudo chown -R `whoami` /opt/gen_logs
* Create soft links for start_logs.sh, tail_logs.sh and stop_logs.sh
  * sudo ln -s /opt/gen_logs/start_logs.sh /usr/bin/start_logs.sh
  * sudo ln -s /opt/gen_logs/tail_logs.sh /usr/bin/tail_logs.sh
  * sudo ln -s /opt/gen_logs/stop_logs.sh /usr/bin/stop_logs.sh
