# Example Docksal addon

This is an example of a Docksal addon. It's purpose is to show a sample folder structure and concepts of creating addons.

## Folder structure

### Name

Addon name is the name of the folder containing it. In this case addon name is `example`.

### Required files

Each addon should have a main script that is named after the addon. In this case script name should be `example` and it should be placed in this folder. An addon will fail to install without the main script.

### Hooks

- `pre-install` script will get executed before addon installation
- `post-install` script will get executed after addon installation

### Optional files

If there is a need to include more files with addon these files should be placed here and paths to those files should be 
put into `addon_name.filelist`. Subfolders structure will be retained. 

In this case the file `example.filelist` exists and lists one additional file. That file is used in `example hello` command.

