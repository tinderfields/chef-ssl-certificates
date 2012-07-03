## DESCRIPTION

Installs and configures SSL certificates for a node.

This cookbook is inspired by the 37 Signals SSL certificates cookbook.

## REQUIREMENTS

Only tested on Debian 6.0.

## USAGE

SSL certificates are defined in the "certificates" cookbook.

````javascript
{
  "id": "my_ssl_cert",
  "name": "ssl.myapp.com",
  "key": "[raw SSL key]",
  "pem": "[raw SSL pem]"
}
````

To install a SSL certificate on a node, use the SSL certificate definition in
your recipe, like this:

````
ssl_certificate 'ssl.myapp.com'
````
