# lab_5_-202001101-
LAB-5
LANGUAGE USED-PYTHON
TOOL USED-MYPY

HOW MYPY IS INSTALLED

GO TO SETTINGS<COMMAND PROMPT<TYPE-python -m pip install mypy

THERE ARE 2 FILES CONTAINING CODE FILES AND THE SCREENSHOT OF THE ERRORS OF BOTH THE FILES ARE ATTACHED IN THE REPOSITORY.
ONE MAJOR ERROR SHOWING IN THE CODE FILES IS THAT CAN NOT FIND IMPLEMENTATION OR LIBRARY STUB OF THE GIVEN MODULE.
                                          
IN FILE-1,I.E app.py,THERE ARE 9 ERRORS AND ALL THE ERROS SAYS THAT CAN NOT FIND IMPLEMENTATION OR LIBRARY STUB OF THE GIVEN MODULE.
IN FILE-2,I.E app2.py,THERE ARE SIMILAR ERROR LIKE THE ABOVE FILE.THE ERROR MEANS if we are getting a Cannot find implementation or library stub for module error, this means mypy was not able to find the module we Making sure your import does not contain a typo.

1)If the module is a third party library, making sure that mypy is able to find the interpreter containing the installed library.

For example, if we are running your code in a virtualenv, make sure to install and use mypy within the virtualenv. Alternatively, if we want to use a globally installed mypy, set the --python-executable command line flag to point the Python interpreter containing our installed third party packages.

2)We can confirm that we are running mypy from the environment you expect by running it like python -m mypy .... We can confirm that We are installing into the environment we expect by running pip like python -m pip ....

3)Reading the how imports are found section below to make sure we understand how exactly mypy searches for and finds modules and modify how we re invoking mypy accordingly.

4)Directly specifying the directory containing the module we want to type check from the command line, by using the mypy_path or files config file options, or by using the MYPYPATH environment variable. are trying to import, whether it comes bundled with type hints or not. If we are getting this error, try:


                                          
                                          
