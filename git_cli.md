# GIT
```bash
################## Configuração ##################

# Configurar nome de usuário global
git config --global user.name "<your_name>"

# Configurar email global
git config --global user.email "<your_email>"

# Configurar nome de usuário local
git config --local user.name "<your_name>"

# Configurar email local
git config --local user.email "<your_email>"

# Verificar configurações
git config --list


################## Branches ##################
# Criar uma nova branch
git branch <branch_name>

# Alternar para uma branch existente
git checkout <branch_name>

# Criar e alternar para uma nova branch
git checkout -b <branch_name>

# Listar branches locais
git branch

# Listar branches remotas
git branch -r

# Deletar uma branch local
git branch -d <branch_name>

################## Remotes ##################
# Adicionar um remote
git remote add origin <repository_url>

# Listar remotes
git remote -v

# Alterar URL de um remote
git remote set-url origin <new_repository_url>

################## Commit e Push ##################
# Adicionar todos os arquivos ao stage
git add .

# Commitar alterações
git commit -m "Mensagem do commit"

# Enviar alterações para o repositório remoto
git push origin <branch_name>

# Forçar push (usar com cuidado)
git push --force


##################  Pull e Fetch ##################
# Atualizar branch local com alterações do repositório remoto
git pull origin <branch_name>

# Baixar alterações sem aplicá-las
git fetch origin

################## Criar Ambientes de Configuração Separados ##################
# Criar um novo repositório local
git init

# Clonar um repositório remoto
git clone <repository_url>

# Criar um repositório bare (sem working directory)
git clone --bare <repository_url>


################## Outros Comandos Úteis  ##################
# Verificar status do repositório
git status

# Verificar histórico de commits
git log

# Reverter um commit
git revert <commit_hash>

# Resetar mudanças para um commit específico
git reset --hard <commit_hash>
