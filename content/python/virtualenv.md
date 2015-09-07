[virtualenv](https://virtualenv.pypa.io/en/latest/) is a tool that is used to create instanced or seperated Python environments. This is great if you are working on multiple projects, or have users on your system who need different Python packages.
`pip install virtualenv`

After virtualenv is installed we can create our Python environment, the path to Python package can be specfied when the environment is created. Otherwise the default version of Python will be used. Make sure to issue the virtualenv command as the user who will be using the environment.
```
cd /home/user
virtualenv -p /usr/bin/python env
```

Once the virtual environment has been created it will need to be activated for use. In the ~/env/bin directory there is a shell script named activate that needs to be run. You will notice that you enviroment is appended before the shell user prompt. To exit the environment you can simply run deactivate. To delete an virtual environment you can delete the directory that was created.
```
source /home/user/env/bin/activate
deactivate
```

The shebang line which should be present on the first line of a Python script references the version of Python specfied when the virtualenv was created.
`#!/usr/bin/env python` 
