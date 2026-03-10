<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #FF7A2E; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-FF7A2E?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 2: Level 02 → 03, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-02%20%E2%86%92%2003-FF7A2E?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #FF7A2E; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

 
Neste nível, precisei ler um ficheiro cujo nome contém **espaços**: `"spaces in this filename"`.  
O objetivo foi extrair o conteúdo desse ficheiro para avançar para o próximo nível.

---
<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Reforcei competências importantes para trabalhar com ficheiros em Linux:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/reading.png"
       width="18"
       style="margin-right: 8px;">
Como manipular ficheiros com **espaços no nome**  
  <p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/slash.png"
       width="18"
       style="margin-right: 8px;">
Uso de **escape** (`\`) para interpretar nomes corretamente  

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
Alternativa com **aspas** para evitar erros  

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
Importância de confirmar o diretório atual antes de executar comandos  

---
<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Utilizei comandos simples, mas aplicados com precisão:

- `ls` → confirmar a existência do ficheiro  
- `cat` → ler o conteúdo  
- `cat "spaces in this filename"` → leitura usando aspas  
- `cat spaces\ in\ this\ filename` → leitura usando escape  

---
<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>
 
Mantive atenção para não cometer erros típicos deste nível:

<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Tentar ler o ficheiro sem escapar os espaços  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Esquecer de usar aspas quando necessário  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Confundir espaços com múltiplos argumentos  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Assumir que o terminal interpreta nomes automaticamente  

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  

A minha abordagem foi direta:

1. Listei os ficheiros do diretório inicial para confirmar o nome exato.  
2. Identifiquei que o nome continha espaços e exigia tratamento especial.  
3. Testei as duas formas corretas: **escape** e **aspas**.  

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Manipulação%20de%20Ficheiros%20com%20Espaços-FF7A2E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
