# database-connect
A single Package for all the database connectivities  ( E.g : MySQL, MongoDb, Cassandra)

## Release Note - version 0.0.1
Support for Mongodb and Cassandra(Datastax Astra) are available.
Features available:
1. Create database/tables
2. Read tables
3. Update tables
4. Delete records
5. Csv/excel data insertion to the available databases.

### Upcoming Plan - version 0.0.2
Support for Mysql

# How to Use

* [install latest package](https://pypi.org/project/database-connect/)

> * in jupyter notebook -

```python
    !pip install database-connect
```

> * in command prompt -

```python
    pip install database-connect
```

## Database Operations

> * import database_connect module

```python
    import database_connect as connection
```

### Let's Do The Operations

* For MongoDb Operations

```python
   import database_connect as connection

   #create the parameters
   client_url = 'paste_your_mongodb_connection_url'  #should be a string
   database = 'your_database_name' #should be a string
   collection_name = 'your_collection_name' #should be a string

   #let's create the mongo object
   mongo = connection.mongo_operation(client_url=client_url, 
                            database=database,
                            collection_name=collection_name)

```

# requirements_dev.txt we use for the testing

It makes it easier to install and manage dependencies for development and testing, separate from the dependencies required for production.

# difference between requirements_dev.txt and requirements.txt

requirements.txt is used to specify the dependencies required to run the production code of a Python project, while requirements_dev.txt is used to specify the dependencies required for development and testing purposes.

# tox.ini

We use if for the testing in the python package testing against different version of the python

## how tox works tox enviornment creation

1. Install depedencies and packages
2. Run commands
3. Its a combination of the (virtualenvwrapper and makefile)
4. It creates a .tox

# pyproject.toml
it is being used for configuration the python project it is a alternative of the setup.cfg file. its containts configuration related to the build system
such as the build tool used package name version author license and dependencies

# setup.cfg
In summary, setup.cfg is used by setuptools to configure the packaging and installation of a Python projec

# Testing python application

*types of testing*

1. Automated testing
2. Manual testing

*Mode of testing*

1. Unit testing
2. Integration tests

*Testing frameworks*

1. pytest
2. unittest
3. robotframework
4. selenium
5. behave
6. doctest

# check with the code style formatting and syntax(coding standard)

1. pylint
2. flake8(it is best because it containt 3 library pylint pycodestyle mccabe)
3. pycodestyle

* Detailed Documentation: <a href = "https://colab.research.google.com/drive/1FfqXKEBhrCOXAU0DWTKjeJJdEMlECmyl?usp=sharing" > Check Here</a>

* Creator - <a href="https://www.linkedin.com/in/sunny-savita/">
Sunny Savita </a>

For any suggestion, contact me on <a href="mailto: sunny.savita@ineuron.ai">sunny.savita@ineuron.ai</a>.