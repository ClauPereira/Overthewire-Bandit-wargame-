<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #2E71FF; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2E71FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-18%20%E2%86%92%2019-2E71FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2E71FF; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a senha para o próximo nível está armazenada em um arquivo chamado **`readme`** no diretório home.

Entretanto, ao tentar fazer login normalmente via **SSH**, a conexão é **encerrada imediatamente**.  
Isso acontece porque alguém modificou o arquivo **`.bashrc`** para executar um comando que finaliza a sessão automaticamente após o login.

Para resolver o desafio, foi necessário **evitar a execução dos scripts do Bash** e abrir a sessão utilizando **um shell diferente**.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **comportamento de shells no Linux**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png" width="18" style="margin-right:8px;">
Como evitar a execução automática de scripts como <code>.bashrc</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/slash.png" width="18" style="margin-right:8px;">
Uso avançado do comando <code>ssh</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Diferença entre shells como <code>bash</code> e <code>sh</code>
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

- `ssh bandit18@bandit.labs.overthewire.org -p 2220 -t /bin/sh` → iniciar sessão SSH usando um shell diferente  
- `ls` → listar os arquivos do diretório home  
- `cat readme` → visualizar o conteúdo do arquivo com a senha  

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
Tentar acessar o servidor usando apenas o comando SSH padrão
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não perceber que o arquivo <code>.bashrc</code> está encerrando a sessão automaticamente
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não utilizar um shell alternativo para evitar a execução dos scripts do Bash
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

1. Tentar acessar o servidor usando SSH normalmente.  
2. Identificar que a conexão era encerrada imediatamente após o login.  
3. Suspeitar que algum script de inicialização do Bash estava executando um comando `exit`.  
4. Utilizar o SSH especificando **um shell alternativo (`/bin/sh`)** para evitar a execução do `.bashrc`.  
5. Após acessar o sistema com sucesso, listar os arquivos do diretório home.  
6. Ler o arquivo `readme` para obter a senha do próximo nível.

Exemplo de comando utilizado:

```bash
ssh bandit18@bandit.labs.overthewire.org -p 2220 -t /bin/sh
```
<p align="center"> <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-SSH%20%7C%20Shell%20Bypass%20%7C%20.bashrc%20%7C%20Linux%20CLI-2E71FF?style=for-the-badge&logo=gnubash&logoColor=white" /> </p>
