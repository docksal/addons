# MailHog

Easily install Mailhog e-mail catcher for your Docksal project

```bash
fin addon install mailhog
```

## Usage once installed

- `fin mailhog disable` to disable
- `fin mailhog enable` to re-enable

## URL

After the installation using the default `*.docksal` domain name, MailHog will be available at `http://webmail-<project_name>.docksal`.



## Regressions
 Previously the url for MailHog could be found at `http://webmail.<project_name>.docksal` or `http://mail.<project_name>.docksal`. This change was made to make it easier to use a LetsEncrypt wildcard certificate, as it is only valid for one level of subdomain.
