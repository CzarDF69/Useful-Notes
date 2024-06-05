### Básicos importantes (important basics)
```bash
$ apt-cache search libssl | grep SSL  # buscar e filtrar
$ apt-get install <app>               # Instalar app
$ cat <arq>                           # mostrar conteúdo de arquivo
$ chmod 777 <arquivo>                 # mudar permissão de arquivo
$ chown -R <user>:<user> <arq>        # mudar dono de arquivo
$ mkdir <dir>                         # criar diretório
$ printenv                            # listar variaveis de ambiente
$ ps                                  # mostrar tasks em execução
$ rm <arq>                            # remover arquivo
$ rmdir <dir>                         # remover diretório vazio
$ systemctl status                    # Mostrar situação atual do sistema
$ sudo -s                             # ser root permanente
$ touch <arq>                         # criar ou atualizar arquivo
$ uname - a                           # dados do sistema
$ whoami                              # quem sou eu?
```
### Criar script bash (create bash script)
```bash
$ sudo vi arq.sh
```
Exemplo de conteúdo (example):
```bash
#!/bin/bash        <== linha obrigatória (mandatory)
apt-get update -y
apt-get upgrade -y
```
Alterar permissões (change permissions):
```bash
$ sudo chown -R <user>:<user> arq.sh
$ sudo chmod 755 arq.sh
```
### npm comands
package.json update
```bash
$ npm outdated               # verificar dependências que possuem atualização
$ npm update                 # atualizações de dependências seguras
$ npx npm-check-updates -u   # atualizar dependências para versões mais recentes
$ npm install                # instalar dependências
```
