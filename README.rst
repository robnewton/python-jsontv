=======
jsontv
=======
Intro
-------------
jsontv downloads and generates television data from SchedulesDirect.org
and parses it into python dicts (and lists). Simple usage is as follows:

::

    #!/usr/bin/env python

    from jsontv import SchedulesDirect

    schedule = SchedulesDirect('username', 'password') 

You can see a full example in the ./examples folder of this project.

Usage
-----

There a few cavets with it's current incarnation:

* ScheduleDirect's current JSON API is VERY much in beta. Much could
  change in how data is sent to the client.
* Because ScheduleDirect sends some data as plain text, and others as
  zip files, some functions return dicts or lists, while others return
  generators.


Contributions
-------------

Please feel free to submit commits if you feel like there is a better 
way to do something.


Python Support
--------------

This has been tested on Python 2.7 and Python 3.2.
