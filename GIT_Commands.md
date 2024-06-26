# GIT

### Criar par de chaves SSH
```bash
ssh-keygen -t ed25519 -C "seu@email.com"
```

### Configuração global do GIT
```bash
git config --global user.email "seu@email.com"
git config --global user.name "Seu Nome"
```

### Inicializar diretório do projeto

```bash
git init
git add .
git commit -m "commit inicial"
git branch -M main
git remote add origin git@github.com:seu-usuario-git/repositorio-git.git
git push -u origin main
```
