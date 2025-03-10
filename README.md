## Install

To use this role with zfs features you'll need to install the collection
`community.general`.

```sh
ansible-galaxy collection install community.general
```

## Parameter

- `nginx_ssl_include`: The name of the file to include, e.g.
  `ssl-www.meissner.it.include`
- `nginx_include_other`
  - `yes` will include `server-{{ site }}.include`
  - The name of the filename to include, e.g. `local-mit-php.include`
- `nginx_include_other_template`: The template to use for the include, e.g.
  `vpn-host-nginx.include`. If used `nginx_include_other` should be omitted.
- Set vars like `mit_nginx_site_db_host` in `group_vars/all`
