# DBeaver - Docksal addon

This Docksal addon launches [DBeaver][1] with the connection information from the current project.
DBeaver is a multi-platform database tool that supports popular database engines like MySQL, PostgreSQL, and more. 

This addon tries to detect the database engine and launches DBeaver with the correct connection settings.
Currently, only the following database engines can be detected:

* MySQL
* PostgreSQL

## Installation
The addon can be installed using the following command:

```bash
fin addon install dbeaver
```

## Usage
Run `fin dbeaver` to launch DBeaver with the connection information from the current project. 

```bash
fin dbeaver
```

If the database service name is not `db` or the project has multiple database services, 
a service name can be provided as the first parameter.

```bash
fin dbeaver database_container
```

Note: on macOS AppleScript is used to determine the installation location of DBeaver. 
When running this script for the first time, a pop-up might ask if it's allowed to execute the AppleScript.

[1]: https://dbeaver.io

