<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #FF7A2E; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-FFA12E?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 3: Level 03 → 04, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-03%20%E2%86%92%2004-FFA12E?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #FFA12E; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, precisei encontrar um ficheiro **oculto** dentro do diretório `inhere`.  
O objetivo foi localizar esse ficheiro escondido e ler o seu conteúdo para avançar para o próximo nível.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Reforcei conhecimentos essenciais sobre ficheiros ocultos em Linux:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png"
       width="18"
       style="margin-right: 8px;">
Como visualizar ficheiros ocultos com `ls -a`  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
Diferença entre ficheiros normais e ficheiros iniciados com `.`  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
Navegação consciente entre diretórios  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/reading.png"
       width="18"
       style="margin-right: 8px;">
Leitura de ficheiros ocultos com comandos básicos  

---

<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Usei comandos simples, mas aplicados de forma precisa:

- `ls -a` → listar ficheiros ocultos  
- `cd inhere` → aceder ao diretório correto  
- `cat .oculto` → ler o ficheiro escondido  
- `ls` → confirmar estrutura do diretório  

---

<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Mantive atenção para não cair em armadilhas típicas deste nível:

<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Usar apenas `ls` e não ver ficheiros ocultos  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Procurar no diretório errado  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Ignorar o ponto (`.`) no nome do ficheiro  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Assumir que ficheiros ocultos são especiais ou protegidos  

---
<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  

A minha abordagem foi direta:

1. Acedi ao diretório `inhere`.  
2. Listei todos os ficheiros, incluindo os ocultos, usando `ls -a`.  
3. Identifiquei o ficheiro oculto `.oculto`.  
4. Li o conteúdo com `cat` para obter a password.  
5. Usei a informação para aceder ao próximo nível via SSH.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Ficheiros%20Ocultos%20%7C%20ls%20--a-FFA12E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>

