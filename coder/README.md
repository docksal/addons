# Coder Docksal addon

Easily install [VS Code](https://github.com/cdr/code-server) for your Docksal project.

## Install

  Please make sure you are in your Docksal project and run:
  ```shell
  fin addon install coder
  ```

## Usage

  Once the addon has been installed and working, at any point in project's lifecycle you can use one of these options: enable (if the container is down for any reason), disable and restart.

  ```shell
  fin coder enable|disable|restart
  ```

  You can use the addon locally (project.docksal) or on a Linux server machine with public domains.

  If used locally, coder starts with no password and no SSL certificates.
  If used on a server with public domains, coder starts with an auto generated password and looks for SSL certs. SSL certs are in the form of 'ide-$VIRTUAL_HOST'.


## Installed extensions

  Out of the box, this addon comes with:
  - [GitLens](https://gitlens.amod.io)

  Additional extensions can be easily installed by clicking the Extensions icon in VSCode itself.
