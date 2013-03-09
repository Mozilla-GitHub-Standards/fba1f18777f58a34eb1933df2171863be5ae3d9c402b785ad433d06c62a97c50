# Description

Chief is a simple web interface to assist in the deployment of web applications.

# Installation

1. `git clone git://github.com/jbalogh/chief.git; cd chief`
2. `cp settings.py.dist settings.py`
3. Fill in settings. The "script" will be run in 3 stages:
    1. `/usr/bin/commander $script pre_update`
    2. `/usr/bin/commander $script update`
    3. `/usr/bin/commander $script deploy`
4. Hook up chief.app to mod\_wsgi, gunicorn, etc.

# Requirements

* [Commander](https://github.com/oremj/commander)

# Change Log

* v0.1.1 - adds a logs directory, fixes #2
* v0.1   - tagged to make an rpm for deployments, by @solarce, fixes #1
