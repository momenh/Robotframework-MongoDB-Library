Robotframework-MongoDB-Library
==============================

A library for interacting with MongoDB from RobotFramework.

Uses pymongo.

Notes
-----

This is a fork from the library [Robotframework-MongoDB-Library](https://github.com/robotframework-thailand/robotframework-mongodb-library.git)

main change is that the json string parsing will be chnaged to bson loads method, 
this way all bson functions like (ObjectId, Timestamps ....etc ) will be supported directly without any needs to explicitly parse using bson in robot framwork



License
-------
See LICENSE file for updated license information

Install
-------
You can install by pulling down source and executing the following:

'''
sudo python setup.py install
'''

# Documentation
For the detail keyword documentation. Go to this following link:

https://robotframework-thailand.github.io/robotframework-mongodb-library/

$ pip install -U setuptools wheel
 
$ python setup.py sdist bdist_wheel
 
$ pip install twine 

$ python3 setup.py sdist bdist_wheel

chmod 600 ~/.pypirc

twine upload --repository testpypi dist/*

twine upload --repository pypi dist/*
