# Default ESP Home project Boilerplate

This is a boilerplate that can be used to start esphome projects from scratch with the following guidelines:

## Setup as new project repositories

1. Create a real repository from this template
2. Clone the repository on your development machine
3. Setup a proper venv for python
4. Install esphome and other requirements by running the following command in the main directory

````
pip install -r requirements.rxr
````

## Structure of the esphome project

The project comes with a

- a valid secret.yaml file that enables you to store sensible informaiton like wifi connection details, mqtt credentials etc. -- Just copy the `secrets.yaml.sample` to `secrets.yaml` and start specifying the details
- a templates directory that  contains some base setups:
  - a `base.yaml` which contains the basic configuration without board specifics 
  - a `wemosd1mini.yaml` containing the basic configuration of a wemos D1 mini device 
  
- within the template directory  there are two packages for additional configuration components:
  - to add the webserver to your device
  - to add homeassistant support to your device

- The main directory contains also a basic `device.yaml` which will create you a wemos D1 mini board that is already setup for basic operations. You just have to add your hardware components to this and you should be ready to go.