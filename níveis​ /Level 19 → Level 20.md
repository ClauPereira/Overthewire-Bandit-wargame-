<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #2E48FF; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2E48FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-19%20%E2%86%92%2020-2E48FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2E48FF; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, para obter a senha do próximo nível é necessário utilizar um **binário especial localizado no diretório home** chamado `bandit20-do`.

Esse binário possui permissões **setuid**, o que significa que ele pode ser executado **com os privilégios de outro usuário**, permitindo acessar arquivos que normalmente não estariam disponíveis.

Após utilizar corretamente o binário, é possível acessar o arquivo padrão onde as senhas são armazenadas.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **controle de privilégios no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png" width="18" style="margin-right:8px;">
Funcionamento de **binários com permissões setuid**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Execução de comandos com privilégios de outro usuário
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png" width="18" style="margin-right:8px;">
Acesso a arquivos protegidos no diretório <code>/etc/bandit_pass</code>
</p>

---

<!-- Comandos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
width="70"
style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos utilizados neste nível foram:

- `ls` → verificar os arquivos disponíveis no diretório home  
- `./bandit20-do` → executar o binário setuid  
- `./bandit20-do cat /etc/bandit_pass/bandit20` → executar o comando `cat` com privilégios do usuário **bandit20**

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
Tentar acessar diretamente o arquivo <code>/etc/bandit_pass/bandit20</code> sem permissões
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não executar o binário setuid com o comando desejado como argumento
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Esquecer de executar o binário usando <code>./</code>
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
width="70"
style="margin-right: 12px;">
Raciocínio aplicado
</h1>

A estratégia utilizada foi:

1. Verificar o conteúdo do diretório home com `ls`.  
2. Identificar o binário `bandit20-do`.  
3. Executar o binário sem argumentos para entender como utilizá-lo.  
4. Utilizar o binário para executar o comando `cat` com privilégios elevados.  
5. Ler o arquivo `/etc/bandit_pass/bandit20`, que contém a senha do próximo nível.

Exemplo de comando utilizado:

```bash
./bandit20-do cat /etc/bandit_pass/bandit20
```
<p align="center"> <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-SetUID%20%7C%20Privilege%20Escalation%20%7C%20Linux%20Permissions-2E48FF?style=for-the-badge&logo=gnubash&logoColor=white" /> </p>
