<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EECFF; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EECFF?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <br>

  <!-- Badge 2: Level 15 → 16 -->
  <img src="https://img.shields.io/badge/Nível-15%20%E2%86%92%2016-2EECFF?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior -->
  <hr style="border:1px solid #2EECFF; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a password para o próximo nível deve ser obtida **enviando a senha atual para uma porta específica utilizando criptografia SSL/TLS**.

Diferente do nível anterior, onde a comunicação foi feita com **Telnet em texto simples**, aqui é necessário usar uma **conexão segura criptografada** para se comunicar com o serviço.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Neste desafio pratiquei conceitos importantes de **comunicação segura em redes**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png" width="18" style="margin-right:8px;">
Diferença entre comunicação em **texto simples** e **criptografada**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ssh.png" width="18" style="margin-right:8px;">
Como estabelecer conexões seguras usando **SSL/TLS**
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png" width="18" style="margin-right:8px;">
Utilização do comando <code>openssl s_client</code> para testar serviços seguros
</p>

---

<!-- Comandos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
width="70"
style="margin-right: 12px;">
Comandos Relevantes
</h1>

Os comandos utilizados neste nível incluem:

- `openssl s_client -connect localhost:30001` → conectar ao serviço SSL/TLS  
- Enviar a senha do nível atual após estabelecer a conexão  
- Receber a senha do próximo nível  

> Observação: utilizar `telnet` ou `nc` neste caso **não funciona**, pois o serviço exige comunicação **criptografada via SSL/TLS**.

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
Tentar utilizar <code>telnet</code> ou <code>nc</code> em vez de SSL
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Não perceber que o serviço exige **criptografia TLS**
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Fechar a conexão antes de enviar a senha
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

1. Identificar que a comunicação deveria ser feita utilizando **SSL/TLS**.  
2. Utilizar o comando `openssl s_client` para estabelecer uma conexão segura com a porta **30001**.  
3. Após a conexão ser estabelecida, enviar a senha do nível atual.  
4. Receber como resposta a senha do próximo nível.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-SSL%2FTLS%20%7C%20OpenSSL%20%7C%20Rede%20Segura-2EECFF?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
