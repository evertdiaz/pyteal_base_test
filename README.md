### Install brew
```
cd /opt
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
export PATH=/opt/homebrew/bin:$PATH
export PATH=/opt/homebrew/sbin:$PATH
```

### Instalar python 3
`brew install python3`

## Instalar nodejs
`brew install node`

## Instalar sandbox
`git clone https://github.com/algorand/sandbox`
`./sandbox up`
`./sandbox enter algod`

## Agregar tus archivos al sandbox, debajo de ports
```
volumes:
- type: bind
  source: ../
  target: /data
```