# SensorPush Ansible Playbooks

Basic Ansible Playbooks to interact with the API provided by sensorpush.com.

# Prerequisites

Obviously, you need a working account with sensorpush.com.\
That you get when you buy the SensorPush Gateway product. See 'Context' below for more information.

# Playbooks

## sensorpush_basic_test_1.yaml

This Playbook will prompt the user for credentials if run with no inventory or parameters:
```
ansible-playbook sensorpush_basic_test_1.yaml
```

If you search for something less interactive, use this:
```
ansible-playbook sensorpush_basic_test_1.yaml -e 'username=<account_e-mail>' -e 'password=<account_password>'
```
or write that information into your inventory.

# Context

The sensors can be used with the App, no strings attached. That was the main feature that made me buy them!\
In order to manage multiple sensors without your phone/tablet becoming the central collection point, you need the SensorPush Gateway.\
With the Gateway, sensor data is pushed to sensorpush.com.
Storage is then managed in the cloud infrastructure and can be checked from anywhere through the phone or the web portal.\
The cloud service comes at no charge (at least as of now).
