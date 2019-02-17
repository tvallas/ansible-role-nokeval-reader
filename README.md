Ansible Role nokeval_reader
=========

This role is used to install and configure nokeval_reader. Typical install target is Raspberry Pi.

Requirements
------------

None

Role Variables
--------------
#### `nokeval_reader_key` (required)
Enter your key here

#### `nokeval_reader_id`: (required)
Enter your client id here

#### `nokeval_reader_required_packages` (optional)
A list of packages required by the role

#### `nokeval_reader_repo_line`: (optional)
Source repo for nokeval_reader packages

#### `nokeval_reader_package` (optional)
Nokeval_service user

#### `nokeval_reader_package_state` (optional)
This variable can be used to update (latest) or remove (absent) reader packages. Default value is present

#### `nokeval_reader_device`: (optonal)
Serial port of the device, default is /dev/ttyUSB0

#### `nokeval_reader_baud` (optional)
Serial port baud rate, default is 9600


Dependencies
------------
None

Example Playbook
----------------

    - hosts: raspberry
      roles:
         - { role: nokeval_reader, nokeval_reader_key: <key here>, nokeval_reader_id: <client id here> }

License
-------

MIT

Author Information
------------------
Tuomas Vallaskangas
tvallas@iki.fi
