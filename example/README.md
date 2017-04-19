# Example Docksal addon

This is an example of an installable Docksal addon. It's purpose is to show a sample folder structure and concepts of creating installable addons.

## Name

Addon name is the name of the folder containing it. In this case addon name is `example`.

## Required files

Each addon should have a main script that is named after the addon. In this case the script name should be named `example` and it should be placed in this folder. An addon will fail to install without the main script.

## Optional files

If there is a need to include more files or use hooks, then these files should be described in `addon_name.filelist` one file per line. 

See contents of `example.filelist` for details.

### Hooks

Hooks scripts should be named as `addon_name.hook_name` and described in `addon_name.filelist`. These scripts are executed automatically upon certain events.

Supported hooks:

- `pre-install` executed before installation, can cancel installation if returns non-zero exit code
- `post-install` executed after installation
- `pre-uninstall` executed before uninstallation, can cancel uninstallation if returns non-zero exit code
- `post-uninstall` executed after uninstallation
