# Example Docksal addon

This is an example of an installable Docksal addon. It's purpose is to show a sample folder structure and concepts of creating installable addons.

## Name

Addon name is the name of the folder containing it. In this case addon name is `example`.

## Required files

Each addon should have a main script that is named as the addon. In this case the main script name is `example`. It should be located in this directory.

## Optional files

If there is a need to include more files, then these files should be described in `addon.filelist` one file per line. 

See contents of `example.filelist` for details.

### Hooks

Hooks are special additional files that executed automatically upon certain events. Hook files should be named as `addon`.`hook` and described in `addon.filelist`.

Supported hooks:

- `pre-install` executed before installation, can cancel installation if returns non-zero exit code
- `post-install` executed after installation
- `pre-uninstall` executed before uninstallation, can cancel uninstallation if returns non-zero exit code
- `post-uninstall` executed after uninstallation

Examples of all these hooks can be found here.
