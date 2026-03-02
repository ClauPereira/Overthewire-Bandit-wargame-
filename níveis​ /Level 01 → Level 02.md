# 🟩 Level 01 → Level 02

<p align="center">
  <img src="https://img.shields.io/badge/Nível-00%20%E2%86%92%2001-1E90FF?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---
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

- 📄 Como lidar com ficheiros cujo nome começa com **caracteres especiais**  
- 🧩 Diferença entre argumentos de comandos e nomes de ficheiros  
- 🐚 Como indicar explicitamente um caminho para evitar interpretações erradas do terminal  
- 🔍 Atenção ao contexto do diretório atual  

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
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Manipulação%20de%20Ficheiros%20Especiais-2E8B57?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
