# Configurações básicas do Git

## 1. Instalação
- [GitForWindows](https://gitforwindows.org/)
- [VS Code](https://code.visualstudio.com/)

## 2. Config
Após a instalação é necessário realizar a sua primeira configuração, neste caso, identificando o nome e o e-mail de quem estará atrelado as alterações.
```
git config --global user.name "Nome Sobrenome"
git config --global user.email "seu_email@example.com"
```

## 3. Init
```
git init
git add . 
git commit -m "Comentário a ser adicionado"
git push
```

## 4. Atualizar o repositório local
Ao utilizar diferentes locais para trabalho se faz necessário sua atualização sempre que for dar início, pois, pode ser que as alterações realizadas não tenho sido baixadas na máquina local.
```
git pull
```

## 5. Copiar um repositório existente
```
git clone <link-repositorio>
```

## 6. Excluir as credenciais
Você pode excluir as credenciais usando uma das opções abaixo.

### 6.1 Credenciais do Windows

![image](https://github.com/user-attachments/assets/6ce5396a-5545-44d5-ad9b-2654a6e3447e)

![image](https://github.com/user-attachments/assets/16660faf-4b3e-4acd-8b42-46e1203d46e4)

### 6.2 Pelo Prompt de Comando (CMD) ou PowerShell

Isso possibilita excluir as credenciais de outra pessoa para que você possa realizar o acesso com seu login e atribuir o seu usuário e e-mail vinculado ao seus commits.

> Lembra de executar esses comandos principalmente se o computador que você geralmente utiliza é compartilhado com outras pessoas.

```
cmdkey /delete:LegacyGeneric:target=git:https://github.com
git config --global --unset-all user.mail
git config --global --unset-all user.email
```

**7.6** Para utilizar basta apenas acessar alguma pasta e clicar com o botão direito. Irá notar que irá aparecer a opção `Open Git Bash`. 

<div align="left">
  <img src="https://github.com/user-attachments/assets/d0c36ce4-09f5-4059-a5e7-8a385440f776" width="50%" />
</div>

> Nota que estou utilizando o Windows 11.


