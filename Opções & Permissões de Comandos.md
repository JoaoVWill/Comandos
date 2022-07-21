# Opções & Permissões de Comandos
### Descrição
*Este é um sub-repositório de* **[COMANDOS_DEBIAN](https://github.com/jvwill/Comandos/blob/main/COMANDOS%20-%20DEBIAN.md)** *com tabelas sobre permissões e opções de cada comando possível*

#

**CHMOD**
  | Opções | Função |
  | --- | --- |
  | -v / --verbose | Mostra todos os arquivos que estão sendo processados |
  | -f / --silent | Não mostra a maior parte das mensagens de erro |
  | -c / --change | Mostra os arquivos que tiveram as permissões alteradas |
  | -R / --recursive | Muda permissões de acesso do ```diretório/arquivo``` no diretório atual e sub-diretórios |

**GPASSWD**
  | Opções | Função |
  | --- | --- |
  | -r | Remove a senha de grupo |
  | -R | Desativa o acesso do grupo usando o comando ```newgrp``` |
  | -a | Adiciona o usuário no grupo especificado |
  | -d | Apaga o usuário do gurpo especificado |
  | -A | Define que o ```usuário``` será o administrador do ```grupo``` |
  | -M | Define os ```usuários``` que fazem parte do ```grupo e suas permissões``` |
  
**CHGRP**
  | Opções | Função |
  | --- | --- |
  | -c / --changes | Somente mostra os ```arquivos/grupos``` que forem alterados |
  | -f / --silent | Não mostra mensagens de erro para ```arquivos/diretórios``` que não puderam ser alterados |
  |-v / --verbose | Mostra todas as ```mensagens e arquivos``` sendo modificados |
  | -R / --recursive | Altera os grupos de ```arquivos/sub-diretórios``` do diretório atua |
