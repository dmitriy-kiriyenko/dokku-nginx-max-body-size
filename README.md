# dokku-nginx-max-body-size
A plugin for Dokku to config max file upload size

## Installation

On a remote server:

```console
$ cd /var/lib/dokku-alt/plugins
$ git clone https://github.com/dmitriy-kiriyenko/dokku-nginx-max-body-size.git
```

No need to install.

## Usage

Add a configuration variable `MAX_UPLOAD_SIZE` with a value in Nginx format.

```console
$ dokku config your-app MAX_UPLOAD_SIZE=100M
```

If you remove this variable, `client-max-body-size` will get back to default value.
