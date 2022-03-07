Project Ncovid 
####################

This page contains the documentation for the Ncovid project. The Ncovid project is an initiative from Prof. Luiz Marcos from UFRN to foment the development of human research for epidemiology forecast, motivate by the COVID-2019 pandemic.

The Ncovid framework is a set of libraries that enables rapid development and deployment of forecast models for epidemics in general. It's main components are the webpage and the backend libraries. The site provides visualization and allow the training of models. You can check the latest version of the ncovid webpage `here <http://ncovid.natalnet.br>`_.

In this page documents both the current and expected versions of the ncovid system.


Main features of the ideal system
*********************************************

In its ideal form the ncovid system allow users to perform the whole ml pipeline to create optimal forecast system for the intended pandemic. This requires:

- Data aggregation
   - Automatic update of the databases;
   - Allow the user to Upload data
- Visualization
   - Show important curves for the selected regions
   - Show many levels of granularity (country, state, cities, etc)
- Train and evaluate forecast models
   - Allow many techniques
   - multiple evaluation metrics
   - Automatic evaluation
- Show forecasts
   - From pre-trained models
   - Show metrics that indicates the models accuracy (degree of confidence)
- Data processing from the pandemic
   - Correlation indices
   - data cleaning
- Configure the parameters of the forecast model
   - type, hyperparameters, inputs, window of forecast, etc..
- Simulate the effects that actions have over the features (doing X, Y, Z can reduce the death tool by alpha)

These are some of the requirements of the system in its full form.

.. note::

   This project is under active development.

Contents
--------

.. toctree::

   pages/terminology
   pages/data_aquisiton
   pages/data_processing
   pages/forecast
   pages/visualization

