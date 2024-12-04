Ansible Role: Intel_SGX_SDK
=========

Ansible Role to install the Intel SGX SDK as described in the Intel SGX Software Installation Guide For Linux OS

Requirements
------------

Pre-requisites not be covered by Ansible or the role:
- None

Role Variables
--------------

The variables defined in `defaults/main.yml` file describe the base URL for the SDK installer and the download as well as install directory.

The entries in `vars/main.yml` can be used to change the SDK version that will be installed

Dependencies
------------

Roles hosted on Galaxy and their parameters:
- None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: melhindi.intel_sgx_sdk }

License
-------

Apache 2.0

Contribute
-------

To contribute to the development of this role the following setup is recommended:

```
# 1. Clone the repository with the expected role name:
git clone git@github.com:melhindi/ansible-role-intel-sgx-sdk.git melhindi.intel_sgx_sdk

# 2. Initialize the virtual environment
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt

# 3. Use molecule to test the role
molecule converge
```
*Note*: This setup assumes that you do not have any globally installed ansible or molecule. Sometimes globally installed ansible/molecule can cause package/dependency conflicts.
