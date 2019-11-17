# EMS Simulator Demos

A sample project that displays two simple working examples of the [EMS Simulator library](https://github.com/EMSTrack/EMS-Simulator). You may use the binder link below to access a Jupyter notebook to play around, or clone this repo and install the packages in requirements.txt manually.

# Examples

## Minimal

The minimal example defines the following setup:

Resources
- 6 pre-defined bases and 2 pre-defined hospitals (directly in the YAML config) in the San Diego area
- Each base hosts a single operational ambulance

Travel Times
- Travel times between locations in the city are randomly selected between 10 and 20 minutes

Cases
- 100 cases will occur randomly within a 2 kilometer circular radius in the San Diego area
- Time interval between incidents is uniformly selected to be between 8 to 18 minutes.

Policies
- A randomly selected available ambulance will attend to the next emergency

## Simple

Resources
- Base and hospital defintions are sourced from an external CSV file
- 5 pre-defined bases and 3 pre-defined hospitals in the San Diego area
- Each base hosts a single operational ambulance

Travel Times
- An external CSV file maps the travel times between each of 600 origin points to each of 600 destination points. Computing travel time between point A and point B involves finding the closest origin to point A, finding the closest destination to point B, and retrieving the corresponding time.

Cases
- Cases are sourced from an external CSV file
- 500 cases will occur randomly within a 2 kilometer rectangular area in the San Diego area
- Time interval between incidents is uniformly selected to be between 8 to 18 minutes.

Policies
- A randomly selected available ambulance will attend to the next emergency

## Run on binder

Demo notebooks can be run online on [binder](https://mybinder.org). 

Just click on the binder logo:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EMSTrack/EMS-Simulator-Demos/master)
