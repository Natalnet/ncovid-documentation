Overview of the Ncovid system
#############################

The frontend of the system is mainly to support of the webpage. The frontend is composed of many modules: the Datamanager module, locales module, and the webpage itself.

The backend performs the ML pipeline, data processing, models training and evaluation. The main models of the backend are: ML modules.

Communication between front and backend is done with REST API.

The system has code in Java, Python and Php.

This system is initially used with data from the COVID-19, but we tried to design an scalable and ease to maintain system, that can easily evolve to be used in other types of pandemics.

To support the requirements of ML pipeline (MLops).

The modules from the system run in containers.

Frontend
********

The frontend is responsible to get and show information to users.

Webpage - Ncovid Hub
====================

The webpage is an essential part of the system. It provides the interface to data visualization of COVID-19 statistics and the forecast from our prediction models. It uses the Laravel framework and requires PHP 7.3. More details `here <https://github.com/Natalnet/ncovid-hub>`_.

Datamanger module
=================

The Datamanger module is a set of libraries used to manage storage and control access to raw data files provided by external repositories. It basically aggregates the necessary raw data used in the training of our forecast models. The files are then assigned a identification key and stored locally in our servers.

An initial pre-processing of the data is performed by this module, to guarantee a minimal structure of the data for later use. The files are then stored in the CSV format, and the information from all the columns (features) are semantically described.

Since the external repositories provides raw data, normally only conditioned to a CSV format, another module is necessary to further pre-process the data for the ML pipeline. More details `here <https://github.com/Natalnet/np-datamanager>`_.


Locales module
==============

This modules provides a service to get the appropriate names for each Country sublocality. This information is then subsequently used by the Datamanager module to get information not only about the country but also its regions, where usable data is available.


Backend
*******

The backend performs all the necessary operations of the ML pipeline, from data processing to forecast models.


ML modules library
==================

NCovid ML Modules is a standalone library for machine learning applications, compatible with receiving requests as web-point. It uses REST API routes to receiving and send requests to the frontend. The libraries perform the whole ML pipeline, from processing raw data, training and evaluation of models.

The code structure is loosely based on the codes from the book `Deep Learning for Time Series Forecasting
Predict the Future with MLPs, CNNs and LSTMs in Python <https://machinelearningmastery.com/deep-learning-for-time-series-forecasting/>`_, by Jason Brownlee.


Communication: REST API
***********************

The REST API is the interface communication between the modules of the system.


A simple data flow
******************

