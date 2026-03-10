<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EFFB8; width:40%; margin:auto 0 8px 0;">
  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EFFB8?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 2: Level 13 → 14, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-13%20%E2%86%92%2014-2EFFB8?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #2EFFB8; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a senha para o próximo nível não é fornecida diretamente.  
O objetivo é utilizar a **chave privada SSH** fornecida para fazer login como o usuário **bandit14** e acessar o arquivo `/etc/bandit_pass/bandit14`, que contém a senha.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Neste desafio, pratiquei conceitos essenciais de **autenticação SSH com chaves privadas**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png" width="18" style="margin-right:8px;">
Como utilizar uma chave privada SSH para autenticação (RSA)
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Estrutura correta de um comando `ssh` com a opção `-i` para chave privada
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png" width="18" style="margin-right:8px;">
Arquivos protegidos no Linux e permissões de acesso (somente usuário proprietário)
</p>

---

<!-- Comandos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
width="70"
style="margin-right: 12px;">
Comandos Relevantes
</h1>

O comando principal utilizado neste nível foi:

- `ssh -i sshkey.private bandit14@localhost` → conecta usando a chave privada  
- `cat /etc/bandit_pass/bandit14` → visualiza a senha (após login)  

> Nota: O parâmetro `-i` do `ssh` indica o **arquivo de identidade**, ou seja, a chave privada usada para autenticação.

---

<!-- Erros comuns -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
width="70"
style="margin-right: 12px;">
Erros comuns evitados
</h1>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Esquecer de definir permissões corretas na chave privada (`chmod 600 sshkey.private`)
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Tentar login com usuário ou host incorreto
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Ignorar a necessidade de usar o arquivo de chave privada
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
width="70"
style="margin-right: 12px;">
Raciocínio aplicado
</h1>

Minha abordagem foi objetiva:

1. Recebi a **chave privada SSH** fornecida para o nível.  
2. Ajustei as permissões da chave para leitura segura: `chmod 600 sshkey.private`.  
3. Usei `ssh -i sshkey.private bandit14@localhost` para me conectar como o usuário **bandit14**.  
4. Naveguei até o arquivo `/etc/bandit_pass/bandit14` e usei `cat` para ler a senha.  

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-SSH%20%7C%20Chave%20Privada-2EFFB8?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
