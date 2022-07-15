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
##

### *Início*
***Comandos de uso comum e diário***

1. Instalação de pacotes [^1]
```ruby
apt install [NOME_DO_PACOTE] 
```
[^1]:Conhecido como gereciador de pacotes, pode ser substituido por outros gereciadores ```yum,pacman```

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

### *USUÁRIOS*
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

6. Adicionar Usuário ao Grupo
- Criar já o usuário dentro de um grupo
```ruby
adduser [Nome_do_Usuário][Grupo]
```
- Criar um grupo já com um usuário
```ruby
addgroup [Nome_do_Usuário][Grupo]
```
- Adicionar de maneira comum
```ruby
gpasswd -a [Nome_do_Usuário][Grupo]
```
```ruby
usermod -a -G [Grupo][Nome_do_Usuário]
```
