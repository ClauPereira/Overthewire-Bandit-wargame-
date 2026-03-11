<div align="center">

  <!-- Linha separadora superior -->
  <hr style="border:1px solid #2EC3FF; width:40%; margin:auto 0 8px 0;">
  <!-- Badge principal -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EC3FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge nível -->
  <img src="https://img.shields.io/badge/Nível-16%20%E2%86%92%2017-2EC3FF?style=for-the-badge&logo=linux&logoColor=white"
       style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2EC3FF; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, as credenciais para o próximo nível estão disponíveis **em uma das portas entre 31000 e 32000 no localhost**.

O desafio consiste em **descobrir qual porta possui um serviço ativo**, verificar **qual delas utiliza SSL/TLS** e então enviar a senha atual para receber **uma chave SSH privada**, que permitirá o acesso ao próximo nível.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio pratiquei conceitos importantes de **análise de portas e serviços em rede**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/port.png" width="18" style="margin-right:8px;">
Como **escanear portas** usando o comando <code>nmap</code>
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png" width="18" style="margin-right:8px;">
Como identificar serviços que utilizam **SSL/TLS**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Como utilizar uma **chave privada SSH** para autenticação
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

- `nmap -p 31000-32000 localhost` → escanear as portas disponíveis  
- `nmap -A -p 31000-32000 localhost` → identificar serviços e verificar suporte a SSL  
- `openssl s_client -connect localhost:31790` → conectar ao serviço SSL correto  
- `chmod 400 <arquivo_chave>` → ajustar permissões da chave privada  
- `ssh -i <arquivo_chave> bandit17@localhost` → acessar o próximo nível usando a chave

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
Tentar testar manualmente todas as portas sem usar um scanner
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não verificar se o serviço utiliza SSL
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não ajustar as permissões da chave privada SSH
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

1. Escanear as portas entre **31000 e 32000** utilizando `nmap`.  
2. Identificar qual porta possui um serviço ativo.  
3. Confirmar se o serviço suporta **SSL/TLS**.  
4. Conectar ao serviço usando `openssl s_client`.  
5. Enviar a senha do nível atual para receber **uma chave privada SSH**.  
6. Salvar a chave em um arquivo e ajustar suas permissões com `chmod 400`.  
7. Utilizar a chave para acessar o próximo nível via SSH.

Exemplo de comando utilizado:

```bash
nmap -A -p 31000-32000 localhost
```

<p align="center">
<img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Port%20Scanning%20%7C%20Nmap%20%7C%20SSL%2FTLS%20%7C%20SSH-2EC3FF?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
