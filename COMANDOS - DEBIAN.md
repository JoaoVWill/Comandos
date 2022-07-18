# <img align="center" alt="Debian" height="70" width="70" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/debian/debian-plain-wordmark.svg" /> Comandos Debian

### Descrição

  Repositório ```.md``` reservado para armazenar comandos gerais do Linux - Debian 
  *podem funcionar em outro sistemas de base Linux ou não*

##  

#### *Informações*

- O comando que tiver o "vim" poderar ser substituido pelo editor de texto que você tiver em sua máquina;
- Aqui eu irei colocar os comandos e suas "tag";
- Certos comandos teram detalhes aqui ou com link redirecionando para um repositório correspondente;

#### *Tópicos*
  Aqui alguns tópicos para se guiar pelo repositório
- [INÍCIO](https://github.com/jvwill/Comandos/blob/main/COMANDOS%20-%20DEBIAN.md#in%C3%ADcioo)
- [USUÁRIOS](https://github.com/jvwill/Comandos/blob/main/COMANDOS%20-%20DEBIAN.md#usuários)
- [GRUPOS](https://github.com/jvwill/Comandos/blob/main/COMANDOS%20-%20DEBIAN.md#grupos)
- [DIRETÓRIOS](https://github.com/jvwill/Comandos/blob/main/COMANDOS%20-%20DEBIAN.md#grupos)
##

### Início
***Comandos de uso comum e diário***

1. Instalação de pacotes [^1]
[^1]:Conhecido como gereciador de pacotes, pode ser substituido por outros gereciadores ```yum,pacman```
```ruby
apt install [NOME_DO_PACOTE] 
```

[LISTA DE PACOTES](https://github.com/Jv2205/Comandos/blob/main/Pacotes%20Linux.md)

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
passwd
```

5. Vizulizar usuários
```ruby
cat /etc/passwd
```

6. Adicionar usuário a um grupo
   - Criar usuário dentro de um grupo [^2]
   [^2]:É necessário criar um grupo antes de executar este comando
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
  
8. Dar permissão de um diretório/arquivo a um usuário
  ```ruby
  chmod [CAMINHO_ABSOLUTO_DO_DIRETÓRIO/ARQUIVO]
  ```
  
9. Tornar usuário dono de um diretório
  ```ruby
  chown [USUÁRIO].[GRUPO_DO_USUÁRIO] [CAMINHO_ABSOLUTO_DO_DIRETÓRIO/ARQUIVO]
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
  groups (USUÁRIO)
  ```
### DIRETÓRIOS
***comandos relacionados a manipulação de Diretórios***
