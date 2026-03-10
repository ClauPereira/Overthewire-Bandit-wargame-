<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid #FF7A2E; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-FFD12E?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 4: Level 04 → 05, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-04%20%E2%86%92%2005-FFD12E?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #FFD12E; width:40%; margin:auto 0 8px 0;">

</div>

<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, precisei encontrar um ficheiro específico dentro do diretório `inhere`.  
O objetivo era localizar o único ficheiro **legível por humanos**, com **1033 bytes** e **não executável**, e depois ler o seu conteúdo para avançar para o próximo nível.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Aprofundei conhecimentos importantes sobre análise de ficheiros em Linux:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/file.png"
       width="18"
       style="margin-right: 8px;">
Como identificar o tipo de um ficheiro com `file`  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/size.png"
       width="18"
       style="margin-right: 8px;">
Como verificar o tamanho exato de um ficheiro  
  <p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/different.png"
       width="18"
       style="margin-right: 8px;">
Diferença entre ficheiros executáveis e não executáveis  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png"
       width="18"
       style="margin-right: 8px;">
Como filtrar ficheiros com propriedades específicas  

---
<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>
Usei comandos essenciais para localizar o ficheiro correto:

- `ls` → listar ficheiros  
- `cd inhere` → aceder ao diretório  
- `file ./-file*` → identificar ficheiros legíveis por humanos  
- `du -b` → verificar tamanho em bytes  
- `cat -file07` → ler o conteúdo do ficheiro certo  

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
Assumir que todos os ficheiros são legíveis  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Ignorar o tamanho exato exigido (1033 bytes)  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Tentar abrir ficheiros binários  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Esquecer de usar `file` para confirmar o tipo de conteúdo  

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  

A minha abordagem foi clara e direta:

1. Acedi ao diretório `inhere`.  
2. Listei os ficheiros e usei `file` para identificar qual era legível por humanos.  
3. Verifiquei o tamanho com `du -b` para confirmar os **1033 bytes**.  
4. Identifiquei o ficheiro correto: **`-file07`**.  
5. Li o conteúdo com `cat` e utilizei a password para avançar para o próximo nível.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Análise%20de%20Ficheiros%20%7C%20file-FFD12E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
