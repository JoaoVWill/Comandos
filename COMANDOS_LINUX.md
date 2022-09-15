# <img align="center" alt="Jv-Linux" height="50" width="50" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg"> Comandos Linux - Debian <img align="center" alt="Debian" height="70" width="70" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/debian/debian-plain-wordmark.svg">

### Descrição

  Repositório ```.md``` reservado para armazenar comandos gerais e de uso diário no Linux - Debian 
  *alguns podem funcionar em outros sistemas de base Linux ou não*

##  

#### *Informações*

- O comando que tiver o "vim" poderar ser substituido pelo editor de texto que você tiver em sua máquina;[^0]
- Aqui eu irei colocar os comandos e suas `opções & permissões` em outro git;
- Esse git está com vários comandos para tarefas diárias.

#### *Tópicos*
- Aqui alguns tópicos para se guiar pelo repositório
  - [INÍCIO](https://github.com/jvwill/Comandos/blob/Default/COMANDOS_LINUX.md#início)
  - [MÁQUINA](https://github.com/jvwill/Comandos/blob/Default/COMANDOS_LINUX.md#máquina)
  - [USUÁRIOS](https://github.com/jvwill/Comandos/blob/Default/COMANDOS_LINUX.md#usuários)
  - [GRUPOS](https://github.com/jvwill/Comandos/blob/Default/COMANDOS_LINUX.md#grupos)
  - [DIRETÓRIOS](https://github.com/jvwill/Comandos/blob/Default/COMANDOS_LINUX.md#diretórios)

##

### Início
***Comandos de uso comum e diário***

1. Instalação de pacotes [^1]
   - [LISTA DE PACOTES](https://github.com/Jv2205/Comandos/blob/main/Pacotes%20Linux.md)

```ruby
apt install [NOME_DO_PACOTE] 
```

2. Limpar tela
```ruby
clear
```

3. Atualizar terminal
```ruby
bash
```

4. Ver comandos utilizados anteriomente
```ruby
history
```

5. Testar conectividade
```ruby
ping
```

### MÁQUINA
***comando com relação a utilização de sua máquina***

1. Trocar o nome da máquina
```ruby
hostnamectl set-hostname [NOME]
```

2. Reiniciar a máquina [^2]

```ruby
systemctl restart netwoking
```

```ruby
service networkinfg resart 
```

3. Ver caminho absoluto de onde está
```ruby
pwd
```

4. Acessar/configurar interfaces da máquina[^3]

```ruby
vim /etc/network/intefaces
```

5. Ver endereçamento de rede
```ruby
ip add
```

### USUÁRIOS
***comandos relacionados a uso de usuários***

1. Criar usuário
```ruby
adduser [NOME_DE_USUÁRIO]
```

2. Excluir usuário
```ruby
deluser [NOME_DE_USUÁRIO]
```

3. Entrar em outro usuário
```ruby
su [USUÁRIO]
```

```ruby
login [USUÁRIO]
```

4. Trocar senha do usuário
```ruby
passwd [USUÁRIO]
```

5. Vizulizar usuários
```ruby
cat /etc/passwd
```

6. Adicionar usuário a um grupo
   - Criar usuário dentro de um grupo [^4]
   [^4]:É necessário criar um grupo antes de executar este comando
   ```ruby
   adduser [NOME_DO_USUÁRIO][GRUPO]
   ```
   - Criar um grupo já com um usuário
   ```ruby
   addgroup [NOME_DO_USUÁRIO][GRUPO]
   ```
   - Adicionar de maneira comum
   ```ruby
   gpasswd -a [NOME_DO_USUÁRIO][GRUPO]
   ```

7. Deletar usuário de um grupo
  ```ruby
  gpasswd -d [NOME_DO_USUÁRIO][GRUPO]
  ``` 
  
8. Dar permissão de um diretório/arquivo a um usuário[^5]

  ```ruby
  chmod  [opções] [permissões] [DIRETÓRIO/ARQUIVO]
  ```
  
9. Tornar usuário dono de um diretório[^5]
  ```ruby
  chown [opções] [USUÁRIO].[GRUPO_DO_USUÁRIO] [DIRETÓRIO/ARQUIVO]
  ```
  
### GRUPOS
***comandos relacionados a criação e configurações de Grupos***

1. Criar um grupo
  ```ruby
  addgroup [NOME_DO_GRUPO]
  ```
2. Excluir um grupo
  ```ruby
  groupdel [NOME_DO_GRUPO]
  ```
3. Vizualizar grupos criados
  ```ruby
  cat /etc/group
  ```
4. Mostrar grupos que um usuário pertence
  ```ruby
  groups [USUÁRIO]
  ```
5. Mudar o grupo de um diretório/arquivo[^5]
  ```ruby
  chgrp [opções] [grupo] [arquivo/diretório]
  ```
  
### DIRETÓRIOS
***comandos relacionados a manipulação de Diretórios***

<!-- 
Linhas das legendas "[^*]"
-->

[^0]: Vim é o editor de texto mais comum em distribuições linux
[^1]: Conhecido como gereciador de pacotes, pode ser substituido por outros gereciadores ```yum,pacman```
[^2]: o comando `systemctl restart netwoking` pode ser usado parareiniciar serviços, só trocar o *netwoking* pelo nome do pacote
[^3]: Necessário o pacote `vim` instalado
[^4]:É necessário criar um grupo antes de executar este comando
[^5]: as ```opções``` e/ou ```permissões``` estão neste segunte repositório [Opções e Permissões](https://github.com/jvwill/Comandos/blob/Default/Opções%20%26%20Permissões%20de%20Comandos.md)
