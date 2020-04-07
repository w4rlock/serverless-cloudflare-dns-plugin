![serverless](http://public.serverless.com/badges/v3.svg)

## Installation
```bash
npm i -E serverless-cloudflaredns-plugin
```

## Usage

```yaml
plugins:
  - serverless-cloudflare-dns

custom:
  cloudflare:
    disabled: false
    domain: ""

    auth:
      email: ""
      token: ""

    record:
      name: ""
      content: ""
      type: ""                    # Optional, default = CNAME
      proxied: ""                 # Optional, default = true
      proxiable: ""               # Optional, default = true
```


## Command Line support
```bash
$ sls cloudflare record deploy
$ sls cloudflare record update
$ sls cloudflare record remove
$ sls cloudflare record list
$ sls cloudflare record list --all
```
