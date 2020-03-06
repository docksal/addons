# Adminer - Docksal addon

Easily install [Adminer](https://www.adminer.org/) for your Docksal project. Make it easy to access the database and examine directly rather then through the CLI.

Adminer (formerly phpMinAdmin) is a full-featured database management tool written in PHP. It consist of a single file that is required to deploy to the target server. Also see: [Introduction to Adminer video](https://www.youtube.com/watch?v=KutqUc1vJUY)

```bash
fin addon install adminer
```

## URL

After the installation using the default `*.docksal` domain name, Adminer will be available at `http://adminer-<project_name>.docksal`.

## Command line reference

- `fin adminer disable` to disable
- `fin adminer enable` to re-enable

## Customization

You can customize your adminer installation with the following environmental variables.

* `ADMINER_DEFAULT_SERVER=db`
  * **db** is the default database container or hostname to connect to.
* `ADMINER_PLUGINS=tables-filter tinymce`
  * To load [Adminer plugins](https://github.com/vrana/adminer/tree/master/plugins) you can pass a list of filenames. 
* `ADMINER_DESIGN=price`
  * To use a bundled [Adminer design](https://github.com/vrana/adminer/tree/master/designs) you can pass its name. 

## Regressions
 Previously the url for Adminer could be found at `http://adminer.<project_name>.docksal`. This change was made to make it easier to use a LetsEncrypt wildcard certificate, as it is only valid for one level of subdomain.
