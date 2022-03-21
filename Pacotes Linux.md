# LISTA DE PACOTES DO LINUX

Segue uma lista com alguns ```Pacotes``` para instalar no Linux e seus ```Comandos Basícos``` ***(digitar somente o que está em parenteses)***
- VIM **(vim)**
- SSH **(ssh openssh-server)**
- Net-tools **(net-tools)**
- DNS **(dnsutils)**
- Apache 2 **(apache2)**
- Apache 2 Doc **(apache2-doc)**
- Bind9 **(bind9)**
- Bind9 Doc **(bind9-doc)**
- W3m **(w3m)**
- DHCP **(isc-dhcp-server)**
- Proftpd **(proftpd)**

### Comandos dos Pacotes
__VIM__:
1. Configs do VIM:
     ```
     vim /etc/vim/vimrc
     ```
2. Exibir número de linhas:
     ```ruby
     vim /etc/vim/vimrc
     procurar e descomentar "syntax ON"
     escrever "set number" na linha de baixo
     ```
3. Outros comandos:

|  Função               |  Comando                 |
| --------------------- | ------------------------ |
|  Entrar no Insert     |  Tecla "i"               |
|  Sair do Insert       |  Tecla "esc"             |
|  Sair e salvar        |  "wq"                    |
|  Sair sem salvar      |  "q!"                    |
|  Copiar ___linhas___  |  "y + nº de linhas + y"  |
|  Colar ___linhas___   |  "p"                     |

__APACHE 2__:
1. Desabilitar site:
  ```
  a2dissite
  ```
2. Habilitar site:
```
a2insite
```
3. Configurar arquivo Index de maneira simples:
```
echo "Mensagem Index" > /var/www/[Diretório_do_site]/index.html
```

__BIND9__ ***Alguns comandos necessitam do VIM ou editor de texto***
1. Declarar uma zona 
```
vim named.conf.local
```
2. Ver zonas default
```
vim named.conf.default-zone
```

__PROFTPD__ ***Alguns comandos necessitam do VIM ou editor de texto***
1. Configurar o proftpd
```
vim proftpd.conf
```

__NGINX__ ***Alguns comandos necessitam do VIM ou editor de texto***
1. Config. do Nginx
```
vim /etc/nginx/nginx.config
```
