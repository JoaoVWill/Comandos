# ***Comandos***


## Descrição

Alguns detalhes a se falar aqui sobre este repositório:
- O comando que tiver o "vim" poderar ser substituido pelo editor de texto que você tiver em sua máquina;
- Aqui eu irei colocar o básico dos comandos, nenhuma config mais especifica ou mais detalhada;
-  

___Legenda___
- "*": pode ser usado de outra maneira


## Início
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
## Máquina
  ***Comandos relacionada a máquina geral***
  1. Mudar nome da máquina:
  ```ruby
  hostnamectl set-hostname [NOME]
  ```
  
  2. Acessar interfaces ***Necessário VIM ou outro editor de texto***
  ```ruby
  vim /etc/network/intefaces
  ```
  
  3. Reiniciar máquina 
  ```ruby
  systemctl restart networking¹
  service networkinfg resart 
  ```
  (¹: pode ser usado para reiniciar serviços/pacotes se necessário)
