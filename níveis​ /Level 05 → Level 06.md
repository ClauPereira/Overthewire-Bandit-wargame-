<div align="center">

  <!-- Linha separadora superior, centralizada -->
  <hr style="border:1px solid # E6FF2E; width:40%; margin:auto 0 8px 0;">

  <!-- Badge 1: Bandit OverTheWire, menor -->
  <img src="https://img.shields.io/badge/Bandit-OverTheWire-E6FF2E?style=for-the-badge&logo=linux&logoColor=white" style="height:35px; display:block; margin:auto;" />

  <!-- Pequena quebra -->
  <br>

  <!-- Badge 5: Level 05 → 06, mesma cor, menor -->
  <img src="https://img.shields.io/badge/Nível-05%20%E2%86%92%2006-E6FF2E?style=for-the-badge&logo=linux&logoColor=white" style="height:30px; display:block; margin:auto; margin-top:8px;" />

  <!-- Linha separadora inferior, centralizada -->
  <hr style="border:1px solid #E6FF2E; width:40%; margin:auto 0 8px 0;">

</div>





<!-- Resumo -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Summary.png"
       width="70"
       style="margin-right: 12px;">
  Resumo do Desafio
</h1>

Neste nível, precisei localizar um ficheiro específico dentro do diretório `inhere`.  
O objetivo era encontrar um ficheiro **legível por humanos**, com **1033 bytes** e **não executável**, e depois ler o seu conteúdo para avançar para o próximo nível.

---

<!-- Conceitos Aprendidos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/concepts_learned.png"
       width="70"
       style="margin-right: 12px;">
Conceitos Aprendidos
</h1>

Aprofundei competências importantes sobre pesquisa avançada de ficheiros:

<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/search.png"
       width="18"
       style="margin-right: 8px;">
Como filtrar ficheiros com propriedades específicas usando `find`  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/size.png"
       width="18"
       style="margin-right: 8px;">
Como identificar ficheiros pelo tamanho exato em bytes  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/different.png"
       width="18"
       style="margin-right: 8px;">
Diferença entre ficheiros legíveis e binários  
<p style="margin: 0; line-height: 1.2; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/trash.png"
       width="18"
       style="margin-right: 8px;">
Como excluir ficheiros executáveis durante a pesquisa  

---

<!-- Comandos-->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/commands.png"
       width="70"
       style="margin-right: 12px;">
Comandos Relevantes
</h1>

Utilizei comandos essenciais para localizar o ficheiro correto:

- `find -type f -readable ! -executable -size 1033c` → localizar ficheiro com todas as propriedades  
- `find -size 1033c` → alternativa rápida baseada apenas no tamanho  
- `cd inhere` → aceder ao diretório  
- `cat maybehere07/.file2` → ler o ficheiro encontrado  

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
Esquecer de especificar unidades (`c` para bytes)  
<!-- erros-->
<p style="margin: 0 0 14px 0; font-size: 12px; font-weight: normal; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/X.png"
       width="18"
       style="margin-right: 12px;">
Procurar apenas por nome e ignorar propriedades  
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
Não excluir ficheiros executáveis na pesquisa  

---

<!-- Raciocínio aplicado -->
<h1 style="margin: 0 0 14px 0; font-size: 34px; font-weight: 800; display: flex; align-items: center;">
  <img src="https://github.com/ClauPereira/Icons/raw/main/WarGames_Overthewire/Thought_process.png"
       width="70"

## Raciocínio aplicado  

A minha abordagem foi clara e eficiente:

1. Acedi ao diretório `inhere`.  
2. Usei `find` para filtrar ficheiros com as propriedades exigidas.  
3. Identifiquei o ficheiro correto: **`maybehere07/.file2`**.  
4. Li o conteúdo com `cat` para obter a password.  
5. Utilizei a informação para aceder ao próximo nível via SSH.

---

<p align="center">
  <img src="https://img.shields.io/badge/Aprendizagem%20Consolidada-Find%20%7C%20Filtros%20Avançados-E6FF2E?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>
