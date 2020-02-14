# Mkcert

This Docksal addon will install mkcert [generate](https://github.com/FiloSottile/mkcert) in the docksal environment. When a certificate for your project is generated the certificate will be trusted by:

- Firefox (Linux & Mac)
- Chrome & Chromium
- curl & wget
- for $VIRTUAL_HOST as well as \*.$VIRTUAL_HOST

## Installation
The mkcert binary is installed as $HOME/.docksal/bin/mkcert **except** when mkcert is already installed on your system. See installation [instructions](https://github.com/FiloSottile/mkcert#installation).
```bash
fin addon install mkcert -g
```
## Use

This command has to be executed **once** before ```fin project start``` in every project.
```bash
# When you are inside a docksal project
fin mkcert create
```
Note: if you have an already start project you can activate it with:  
```bash
fin project stop; sleep 2; fin project start
```
Open https://[project].docksal (Or your known URL)
