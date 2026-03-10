<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #FF512E; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-FF512E?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 2: Level 01 → 02, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-01%20%E2%86%92%2002-FF512E?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #FF512E; width:40%; margin:auto 0 8px 0;">

</div>


<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, precisei identificar e ler um ficheiro cujo nome é apenas um **caractere especial**: `-`.  
O objetivo era extrair a informação contida nele para avançar para o próximo nível.

---
<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Neste exercício, reforcei competências importantes para manipulação de ficheiros em Linux:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/security.png"
       width="18"
       style="margin-right: 8px;">
Como lidar com ficheiros cujo nome começa com **caracteres especiais**  
 <p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/structure.png"
       width="18"
       style="margin-right: 8px;">
Diferença entre argumentos de comandos e nomes de ficheiros  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
Como indicar explicitamente um caminho para evitar interpretações erradas do terminal  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png"
       width="18"
       style="margin-right: 8px;">  
Atenção ao contexto do diretório atual  

---
<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>
  
Utilizei comandos simples, mas aplicados de forma consciente:

- `ls` → confirmar a existência do ficheiro  
- `cat` → ler conteúdo  
- caminhos relativos (`./`) → evitar conflitos com nomes especiais  

---
<!-- Erros comuns evitados-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/ErrorX.png"
       width="70"
       style="margin-right: 12px;">
Erros comuns evitados
</h1>

Mantive foco para não cair em armadilhas típicas deste nível:

<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Tentar ler o ficheiro `-` sem especificar o caminho  
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Confundir o nome do ficheiro com opções de comando  
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Assumir que todos os ficheiros têm nomes “normais”  
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Ignorar o diretório atual antes de executar comandos  

---
<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  

A minha abordagem foi direta:

1. Listei os ficheiros do diretório inicial para confirmar a presença do ficheiro `-`.  
2. Percebi que o nome poderia ser interpretado como argumento de comando.  
3. Usei o caminho relativo para indicar explicitamente que se tratava de um ficheiro.  
4. Reforcei a importância de compreender como o terminal interpreta nomes e argumentos.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Manipulação%20de%20Ficheiros%20Especiais-FF512E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
