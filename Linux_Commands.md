### Básicos importantes (important basics)
```bash
apt-cache search libssl | grep SSL  # buscar e filtrar
apt-get install <app>               # instalar app
cat <arq>                           # mostrar conteúdo de arquivo
chmod 777 <arquivo>                 # mudar permissão de arquivo
chown -R <user>:<user> <arq>        # mudar dono de arquivo
mkdir <dir>                         # criar diretório
ping6 -c 5 ::1                      # ping para verificar IPv6 habilitado
printenv                            # listar variaveis de ambiente
ps                                  # mostrar tasks em execução
rm <arq>                            # remover arquivo
rmdir <dir>                         # remover diretório vazio
systemctl status                    # mostrar situação atual do sistema
sudo -s                             # ser root permanente
touch <arq>                         # criar ou atualizar arquivo
uname - a                           # dados do sistema
whoami                              # quem sou eu?
```
### Criar script bash (create bash script)
```bash
sudo vi arq.sh
```
Exemplo de conteúdo (example):
```bash
#!/bin/bash        <== linha obrigatória (mandatory)
apt-get update -y
apt-get upgrade -y
```
Alterar permissões (change permissions):
```bash
sudo chown -R <user>:<user> arq.sh
sudo chmod 755 arq.sh
```
### SSH comands
```bash
ssh-keygen                          # criar par de chaves na máquina origem
# --> conectar-se à instância EC2 da AWS
ssh -i ~/.ssh/key.pem ubuntu@ec2-18-190-34-184.us-east-1.compute.amazonaws.com
# --> copiar arquivos
scp -P 22 -i ~/.ssh/key.pem * ubuntu@ec2-3-129-52-42.us-east-1.compute.amazonaws.com:/var/www/pasta_destino
# --> copiar pasta
scp -P 22 -i ~/.ssh/key.pem -r ./pasta ubuntu@ec2-3-129-52-42.us-east-1.compute.amazonaws.com:/var/www/pasta_destino
```
