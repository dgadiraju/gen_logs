# gen_logs

This is to simulate web application writing traffic details to log file.

* It has shell scripts which invoke python program
* It is compatible with Python 2

Here is the setup process on linux or mac or on cygwin.

* Identify directory /opt/
* Copy gen_logs directory to /opt - ```sudo mv -f gen_logs /opt```
* Run ```sudo chown -R `whoami` /opt/gen_logs```
* Update PATH in .profile or .bash_profile or create soft links for the shell programs - ```export PATH=$PATH:/opt/gen_logs```
* Either restart shell or run .profile/.bash_profile script
* Run ```start_logs.sh``` to start generating web logs
* Run ```tail_logs.sh``` to preview while logs are being generated (Hit ctrl-c to come out)
* Run ```stop_logs.sh``` to stop generating web logs
