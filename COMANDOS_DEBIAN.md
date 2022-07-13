# <img align="center" alt="Debian" height="70" width="70" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/debian/debian-plain-wordmark.svg" /> **Comandos_Debian**

### *Descrição*

  Arquivo .md separado para armazenar comandos gerais do Linux Debian 
  *podem funcionar em outro sistemas de base Linux ou não*
  
### *Informações*

Alguns detalhes a se falar aqui sobre este repositório:
- O comando que tiver o "vim" poderar ser substituido pelo editor de texto que você tiver em sua máquina;
- Aqui eu irei colocar o básico dos comandos, nenhuma config mais especifica ou mais detalhada;

##

### *Tópicos*

Aqui os links para chegar no tópico que seja do seu interesse

- [INÍCIO](https://github.com/jvwill/Comandos/blob/main/COMANDOS_DEBIAN.md#in%C3%ADcio)

- [MÁQUINA](https://github.com/jvwill/Comandos/blob/main/COMANDOS_DEBIAN.md#m%C3%A1quina)

- [USUÁRIOS,GRUPOS & DIRETÓRIOS](https://github.com/jvwill/Comandos/blob/main/COMANDOS_DEBIAN.md#usu%C3%A1rios-grupos--diret%C3%B3rios)


## 

### *Início*
  ***Aqui está o mais basíco do Linux:***
  1. Instalação de pacotes: 
  ```ruby
  apt install [NOME_DO_PACOTE]
  ```
  [LISTA DE PACOTES](https://github.com/Jv2205/Comandos/blob/main/Pacotes%20Linux.md)
  
  2. Acessar usuário Root a partir de um usuário comum:
  ```ruby
  su
  ```
  3. Trocar terminal no Debian (Linux):
  
     Alt + seta direita/esquerda __OU__  Alt + f1 até f6
  
  4. Limpar tela
  ```ruby
  clear
  ```
  
  5. Atualizar terminal
  ```ruby
  bash
  ```
##

### *Máquina*
  ***Comandos relacionada a máquina geral***
  1. Mudar nome da máquina:
  ```ruby
  hostnamectl set-hostname [Nome]
  ```
  
  2. Acessar interfaces ***Necessário VIM ou outro editor de texto***
  ```ruby
  vim /etc/network/intefaces
  ```
  
  3. Reiniciar máquina 
  
  ```ruby 
  systemctl restart netwoking
  ```
  ↑ [^1]
  ```ruby
  service networkinfg resart 
  ```
  [^1]: pode ser usado para reiniciar serviços/pacotes se necessário, só substituir `netwoking` pelo nome do pacote

  4. Ver LOG do sistema
  ```ruby
  tail -f -n 100 /var/log/syslog
  ```
  
  5. Pingar *(chamar)* um endereço
  ```ruby
  ping [endereço]
  ```
  
  6. Criar um Backup
  ```ruby
  cp [Arquivo][Nome_do_Backup]
  ```
  
  ##
  
  ### *USUÁRIOS, GRUPOS & DIRETÓRIOS*
   ***aqui os comandos para edição de usuários, grupos e diretórios***
   
  1. Criar Usuários
  ```ruby
  adduser [Nome_do_Usuário]
  ```
  
  2. Excluir Usuários
  ```ruby
  userdel -r [Nome_do_Usuário]
  ```
  
  3. Entrar em outro usuário
  ```ruby
  login [Nome_do_Usuário]
  ```
  
  ```ruby
  su [Nome_do_Usuário]
  ```
  4. Trocar senha de um usuário
  ```ruby
  passwd 
  ```
 
  6. Vizualizar Usuários
  ```ruby
  cat /etc/passwd
  ```
  
  6. Criar um Grupo
  ```ruby
  groupadd [Nome_do_Grupo]
  ```
  ```ruby
  addgroup [Nome_do_Grupo]
  ```
  
  7. Deletar um Grupo
  ```ruby
  groupdel [Grupo]
  ```
  
  8. Vizualizar Grupos
  ```ruby
  cat etc/group
  ```
  
  9. Adicionar Usuário ao Grupo
  ```ruby
  adduser [Nome_do_Usuário][Grupo]
  ```
  ```ruby
  addgroup [Nome_do_Usuário][Grupo]
  ```
  ```ruby
  gpasswd -a [Nome_do_Usuário][Grupo]
  ```
  ```ruby
  usermod -a -G [Grupo][Nome_do_Usuário]
  ```
  
  10. Deletar Usuário do Grupo
  ```ruby
  gpasswd -d [Nome_do_Usuário][Grupo]
  ```
    
  11. Acessar um Diretorio
  ```ruby
  cd /etc/[Caminho]/[Nome_do_Diretorio]
  ```      
  
  12. Criar um Diretorio
  ```ruby
  mkdir -p /mnt/[Nome_do_Diretorio]
  ```
  
  13. Sair do Diretorio
  ```ruby
  cd ..
  ```
   
  14. Criar Usuário/Grupo em um Diretorio
  
  __GRUPO__
  ```ruby
  mkdir -p /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo]
  ```
  __USUÁRIO__
  ```ruby
  mkdir -p /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo]/[Nome_do_Usuário] 
  ```
  
  15. Criar Pasta em um Diretorio
  ```ruby
  chgrp [Nome_da_Pasta_do_Grupo] /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo] [Nome_da_Pasta_do_Grupo]
  ```
  
  16. Dar Permissão para um Grupo/Usuário
  
  __GRUPO__
  ```ruby
  chmod 750 /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo]
  ```
  __USUÁRIO__
  ```ruby      
  chmod 750 /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo]/[Nome_do_Usuário]
  ```
  17. Tornar um Usuário Dono da Pasta
  ```ruby
  chown [Nome_do_Usuário].[Nome_do_Grupo] /mnt/[Nome_do_Diretorio]/[Nome_do_Grupo]/[Nome_do_Usuário]
  ```
  
  ##
  
  ### FIM
