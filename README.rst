Hello Pyramid
=============

This repo houses the sample code used in my `How-To: Hello Pyramid on AWS <http://bruisedthumb.com/post/2017-03-05>`_ Tutorial.

It contains the following

* application.py: the meat of the application
* requirements.txt: the requirements that do work with AWS ElasticBeanstalk.
* requirements_ideal.txt: the requirements that should work, but the python34 build on Amazon Linux is missing wheels.
* deployment.zip: the package that can be uploaded straight to a AWS EB instance and work. 
* ideal.zip: the package that should be uploaded straight to a AWS EB instance but doesn't because of that pesky python34 on Amazon Linux.

Note on Amazon Linux
--------------------

Amazon Linux is derived from Red Hat, and Red Hat has a package policy to avoid including system libraries in a package. This breaks their python34 build. You can read more `here <http://bruisedthumb.com/post/2017-03-20>`_ 
