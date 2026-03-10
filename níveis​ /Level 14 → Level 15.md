<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #2EFFE2; width:40%; margin:auto 0 8px 0;">
  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-2EFFE2?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 2: Level 14 → 15, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-14%20%E2%86%92%2015-2EFFE2?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #2EFFE2; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
width="70"
style="margin-right: 12px;">
Resumo do Desafio
</h1>

Neste nível, a senha para o próximo nível é obtida **enviando a senha atual** para uma porta específica no localhost.  
O objetivo é conectar-se à porta **30000** no servidor local e fornecer a senha do nível 14 para receber a senha do próximo nível.

---

<!-- Conceitos Aprendidos -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
width="70"
style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Durante este desafio, pratiquei conceitos de **comunicação entre hosts via rede**:

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ssh.png" width="25" style="margin-right:8px;">
Como enviar dados para outro host usando o comando `telnet`
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/test.png" width="25" style="margin-right:8px;">
Uso do **localhost (127.0.0.1)** para testes de rede locais
</p>

<p style="margin:0; line-height:1.2; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/port.png" width="18" style="margin-right:8px;">
Como se comunicar com portas específicas em um host
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

- `telnet localhost 30000` → conecta-se à porta 30000 no localhost  
- Enviar a senha do nível 14: `4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`  
- O servidor retorna a senha do nível 15 e encerra a conexão  

> Observação: A conexão Telnet será fechada pelo host após a tentativa de senha.

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
Esquecer de usar a senha correta do nível anterior
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Tentar conectar em uma porta diferente
</p>

<p style="margin:0 0 14px 0; font-size:12px; display:flex; align-items:center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png" width="18" style="margin-right:12px;">
Ignorar o localhost e tentar usar IP externo desnecessariamente
</p>

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
<img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
width="70"
style="margin-right: 12px;">
Raciocínio aplicado
</h1>

Minha abordagem foi:

1. Identificar que a senha do nível 14 estava em `/etc/bandit_pass/bandit14`.  
2. Abrir uma conexão Telnet para `localhost` na porta `30000`.  
3. Enviar a senha do nível 14 para receber a senha do próximo nível.  
4. Analisar a resposta do servidor e registrar a senha do nível 15.  
5. Compreender o padrão: **enviar senha → receber senha do próximo nível** em portas específicas.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Telnet%20%7C%20Portas%20%7C%20Localhost-2EFFE2?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
