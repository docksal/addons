# mkcert

[mkcert](https://github.com/FiloSottile/mkcert) addon for Docksal.

A mkcert generated cert will be trusted locally by:

- Firefox (Linux & Mac)
- Chrome & Chromium
- curl & wget

The cert is automatically generated for `VIRTUAL_HOST` and `*.VIRTUAL_HOST`.

## Installation

```bash
fin addon install --global mkcert
```

The `mkcert` binary is installed in `$HOME/.docksal/bin/mkcert` **except** when `mkcert` is already installed globally. 

## Use

In a project directory, run:

```bash
fin mkcert create
fin project restart
```

Open https://[project].docksal to validate.
