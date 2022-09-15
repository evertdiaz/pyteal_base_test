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
`git clone https://github.com/algorand/sandbox.git`

## Agregar tus archivos al sandbox, debajo de ports
```
volumes:
- type: bind
  source: ../
  target: /data
```

## Levantar el sandbox
`./sandbox up -v`
`./sandbox enter algod`

